1. Navbar

```html
<!DOCTYPE html>
<html>

<head>
  <!--Import Google Icon Font-->
  <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
  <!--Import materialize.css-->
  <link type="text/css" rel="stylesheet" href="css/materialize.min.css" media="screen,projection" />
  <link type="text/css" rel="stylesheet" href="css/main.css" />
  <!--Let browser know website is optimized for mobile-->

  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Custom Materialize Theme</title>
</head>

<body>

<div class="navbar-fixed">
  <nav class="teal">
    <div class="container">
      <div class="nav-wrapper">
        <a href="#home"  class="brand-logo" >Travelville</a>
        <a href="#" data-activates="mobile-nav" class="button-collapse">
          <i class="material-icons">menu</i>
        </a>
          <ul class="right hide-on-med-and-down">
            <li><a href="#home">Home</a></li>
            <li><a href="#search">Search</a></li>
            <li><a href="#popular">Popular Places</a></li>
            <li><a href="#gallery">Gallery</a></li>
            <li><a href="#contact">Contact</a></li>


          </ul>
      </div>
    </div>
  </nav>
</div>



  <ul class="side-nav" id="mobile-nav">
    <li><a href="#home">Home</a></li>
    <li><a href="#search">Search</a></li>
    <li><a href="#popular">Popular Places</a></li>
    <li><a href="#gallery">Gallery</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>


  <!--Import jQuery before materialize.js-->
  <script type="text/javascript" src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
  <script type="text/javascript" src="js/materialize.min.js"></script>
  <script>
    $(document).ready(function () {
      // Custom JS & jQuery here
      $('.button-collapse').sideNav();
      
    });
  </script>
</body>

</html>
```


2. Slider

```html

<!--    section slider-->

    <section class="slider">
        <ul class="slides">
            <li>
                <img src="img/resort1.jpg" alt="">
                <div class="caption center-align">
                  <h2>Take your dream vacation</h2>
                  <h5 class="light grey-text lighten-3 hide-on-small-only">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad consectetur facere nisi soluta veritatis vitae.</h5>
                  <a href="#" class="btn btn-large">Learn More</a>
                </div>
            </li>
          <li>
            <img src="img/resort2.jpg" alt="">
            <div class="caption left-align">
              <h2>We work with all budgets</h2>
              <h5 class="light grey-text lighten-3 hide-on-small-only">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad consectetur facere nisi soluta veritatis vitae.</h5>
              <a href="#" class="btn btn-large">Learn More</a>
            </div>
          </li>

          <li>
            <img src="img/resort3.jpg" alt="">
            <div class="caption right-align">
              <h2>Group and giveaways</h2>
              <h5 class="light grey-text lighten-3 hide-on-small-only">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad consectetur facere nisi soluta veritatis vitae.</h5>
              <a href="#" class="btn btn-large">Learn More</a>
            </div>
          </li>
        </ul>
    </section>


  <!--Import jQuery before materialize.js-->
  <script type="text/javascript" src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
  <script type="text/javascript" src="js/materialize.min.js"></script>
  <script>
    $(document).ready(function () {
      // Custom JS & jQuery here
    // INIT NAV
      $('.button-collapse').sideNav();


      //INIT SLIDER

      $('.slider').slider({
        indicators:false,
        height:500,
        transition:500,
        interval:5500
      })
    });
  </script>
```




3. Search

```html
    <section class="section section-search teal darken-1 white-text center">
      <div class="container">
        <div class="row">
          <div class="s12">
            <h3>Search Destinations</h3>
             <div class="input-field">
               <input class="white grey-text autocomplete" placeholder="Aruba,Cancun,Ibizza" id="autocomplete-input" type="text">
             </div>
          </div>
        </div>
      </div>
    </section>




  <!--Import jQuery before materialize.js-->
  <script type="text/javascript" src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
  <script type="text/javascript" src="js/materialize.min.js"></script>
  <script>
    $(document).ready(function () {
      // Custom JS & jQuery here
    // INIT NAV
      $('.button-collapse').sideNav();


      //INIT SLIDER

      $('.slider').slider({
        indicators:false,
        height:500,
        transition:500,
        interval:5500
      })


      $('.autocomplete').autocomplete({
        data:{
          "Aruba":null,
          "Cancun Mexico":null,
          "Hawaii":null,
          "The bahamas":null,
        }
      });

    });


```




4. Icon boxes

```html


<!--   Section icon boxes-->



  <section class="section section-icons grey lighten-4 center">
    <div class="container">
      <div class="row">
        <div class="col s12 m4">
          <div class="card-panel">
               <i class="material-icons large teal-text">room</i>
            <h4>Pick Where</h4>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus, saepe?</p>
          </div>
        </div>

        <div class="col s12 m4">
         <div class="card-panel">
            <i class="material-icons large teal-text">store</i>
            <h4>Fly</h4>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus, saepe?</p>
          </div>
        </div>

        <div class="col s12 m4">
          <div class="card-panel">
            <i class="material-icons large teal-text">home</i>
            <h4>Travel Shop</h4>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus, saepe?</p>
          </div>
        </div>
      </div>


      </div>
    </div>
  </section>




```



5. Popular locations card with images


```html
<!--  Section :    Popular-->

<div class="section section-popular">
  <div class="container">
    <div class="row">
      <h4 class="center"><span class="teal-text">Popular</span> Place</h4>

      <div class="col 12 m4">
        <div class="card">
          <div class="card-image">
            <img src="img/resort1.jpg" alt="">
            <span class="card-title">Cancun, Mexico</span>
          </div>
          <div class="card-content">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Delectus hic laboriosam omnis qui recusandae.</p>
          </div>
        </div>
      </div>

      <div class="col 12 m4">
        <div class="card">
          <div class="card-image">
            <img src="img/resort2.jpg" alt="">
            <span class="card-title">Vega</span>
          </div>
          <div class="card-content">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Delectus hic laboriosam omnis qui recusandae.</p>
          </div>
        </div>
      </div>


      <div class="col 12 m4">
        <div class="card">
          <div class="card-image">
            <img src="img/resort3.jpg" alt="">
            <span class="card-title">Nova Scotia</span>
          </div>
          <div class="card-content">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Delectus hic laboriosam omnis qui recusandae.</p>
          </div>
        </div>
      </div>



    </div>

    <div class="row">
      <div class="col s12 center">
        <a href="#contact" class="btn btn-large grey darken-3">
          <i class="material-icons left">send</i>Contact for booking
        </a>
      </div>
    </div>

  </div>
</div>



  
```



6. Section follow and image gallery

```html

    <section class="section section-follow teal darken-2 white-text center">
        <div class="container">
          <div class="row">
            <div class="col s12">
              <h4>Follow Travelville</h4>
              <p>Follow us on social media for special offers</p>
              <a href="https://facebook.com" target="_blank" >
                <i class="fab fa-facebook fa-4x"></i>
              </a>

              <a href="https://twitter.com" target="_blank" class="white-text">
                <i class="fab fa-twitter fa-4x"></i>
              </a>


              <a href="https://pinterest.com" target="_blank" class="white-text">
                <i class="fab fa-pinterest fa-4x"></i>
              </a>
              <a href="https://linkedin.com" target="_blank" class="white-text">
                <i class="fab fa-linkedin fa-4x"></i>
              </a>
              <a href="https://googleplus.com" target="_blank" class="white-text">
                <i class="fab fa-google-plus fa-5x"></i>
              </a>
            </div>
          </div>
        </div>
    </section>


<!--  Section gallery-->


  <div class="section section section-gallery">
        <div class="container">
             <h4 class="center">
               <span class="teal-text">Photo</span>Gallery
             </h4>

             <div class="row">
               <div class="col s12 m3">
                 <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?beach" alt="">
               </div>
               <div class="col s12 m3">
                 <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?nature" alt="">
               </div>
               <div class="col s12 m3">
                 <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?travel" alt="">
               </div>
               <div class="col s12 m3">
                 <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?jungle" alt="">
               </div>
             </div>


          <div class="row">
            <div class="col s12 m3">
              <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?resort" alt="">
            </div>
            <div class="col s12 m3">
              <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?forest" alt="">
            </div>
            <div class="col s12 m3">
              <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?elephant" alt="">
            </div>
            <div class="col s12 m3">
              <img class="materialboxed responsive-img" src="https://source.unsplash.com/1600x900/?koala" alt="">
            </div>
          </div>


        </div>
  </div>

```



 **css**
 
```css
.slider .btn{
    margin-top: 20px;
}


.section-search input{
    padding: 5px !important;
    font-size: 18px !important;
    width: 90% !important;
    border: #f4f4f4 3px solid !important;
}

.autocomplete-content{
    position: absolute;
    width: 100%;
    text-align: center;
}

.section-follow .fa-4x {
    margin: 5px 10px;
}

```


# Contact section

```html
<!-- section contact  -->


  <section class="section section-contact">
      <div class="container">
        <div class="row">
          <div class="col s12 m6">
             <div class="card-panel teal white-text center">
                  <i class="material-icons medium">email</i>
               <h5>Contact Us for Booking</h5>
               <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Animi fugit ipsam iste maxime mollitia nostrum odio quisquam sint tempore vitae.</p>

             </div>

            <ul class="collection with-header">
              <li class="collection-header">
                <h4>Location</h4>
              </li>
              <li class="li collection-item">Travelville Agency</li>
              <li class="collection-item">777 CR7 Turin</li>

            </ul>
          </div>
          <div class="col s12 m6">
              <div class="card-panel grey lighten-3">
                <h5>Please fill out this form</h5>
                <div class="input-field">
                  <input type="text" placeholder="Name" id="name">
                  <label for="name">Name</label>
                </div>
                <div class="input-field">
                  <input type="email" placeholder="Name" id="email">
                  <label for="email">Email</label>
                </div>
                <div class="input-field">
                  <input type="text" placeholder="Phone" id="phone">
                  <label for="phone">Phone</label>
                </div>
                <div class="input-field">
                  <textarea class="materialize-textarea" placeholder="Enter message" id="message"></textarea>
                  <label for="message">Message</label>
                </div>

                <input type="submit" value="submit" class="btn">

              </div>
          </div>

        </div>
      </div>
  </section>
```






# Footer section

```html
<!--  Footer -->
<footer class="section teal darken-2 white-text center">
  <p class="flow-text">Travelville &copy; 2019</p>
</footer>
```


**css*

```css
.slider .btn{
    margin-top: 20px;
}


.section-search input{
    padding: 5px !important;
    font-size: 18px !important;
    width: 90% !important;
    border: #f4f4f4 3px solid !important;
}

.autocomplete-content{
    position: absolute;
    width: 100%;
    text-align: center;
}



.section-follow .fa-4x {
    margin: 5px 10px;
}





.section-contact h5 {
    margin-bottom: 30px;
}





```





#  Scroll it!

```html


```