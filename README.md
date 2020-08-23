 <html> 
 <html lang="en"> 
   <head> 
     <meta charset="utf-8"> 
     <meta http-equiv="X-UA-Compatible" content="IE=edge"> 
     <meta name="viewport" content="width=device-width, initial-scale=1"> 
     <title>David Chu's China Bistro</title> 
     <link rel="stylesheet" href="css/bootstrap.css"
     <link rel="stylesheet" href="css/bootstrap.min.css"> 
     <link rel="stylesheet" href="css/styles.css"> 
     <link href='https://fonts.googleapis.com/css?family=Oxygen:400,300,700' rel='stylesheet' type='text/css'> 
     <link href='https://fonts.googleapis.com/css?family=Lora' rel='stylesheet' type='text/css'> 
   </head> 
 <body> 
   <header> 
     <nav id="header-nav" class="navbar navbar-default"> 
       <div class="container"> 
         <div class="navbar-header"> 
           <a href="index.html" class="pull-left visible-md visible-lg"> 
             <div id="logo-img" alt="Logo image"></div> 
           </a> 
            <div class="navbar-brand"> 
            <a href="index.html"><h1>David Chu's China Bistro</h1></a> 
             <p> 
               <img src="images/star-k-logo.png" alt="Kosher certification"> 
               <span>Kosher Certified</span> 
             </p> 
           </div> 
          <button id="navbarToggle" type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#collapsable-nav" aria-expanded="false"> 
             <span class="sr-only">Toggle navigation</span> 
             <span class="icon-bar"></span> 
             <span class="icon-bar"></span> 
             <span class="icon-bar"></span> 
           </button> 
         </div> 
           <div id="collapsable-nav" class="collapse navbar-collapse"> 
            <ul id="nav-list" class="nav navbar-nav navbar-right"> 
             <li id="navHomeButton" class="visible-xs active"> 
               <a href="index.html"> 
                 <span class="glyphicon glyphicon-home"></span> Home</a> 
             </li> 
             <li id="navMenuButton"> 
               <a href="#" onclick="$dc.loadMenuCategories();"> 
                 <span class="glyphicon glyphicon-cutlery"></span><br class="hidden-xs"> Menu</a> 
             </li> 
             <li> 
               <a href="#"> 
                 <span class="glyphicon glyphicon-info-sign"></span><br class="hidden-xs"> About</a> 
             </li> 
             <li> 
               <a href="#"> 
                 <span class="glyphicon glyphicon-certificate"></span><br class="hidden-xs"> Awards</a> 
             </li> 
             <li id="phone" class="hidden-xs"> 
               <a href="tel:410-602-5008"> 
                 <span>410-602-5008</span></a><div>* We Deliver</div> 
             </li> 
           </ul><!-- #nav-list --> 
         </div><!-- .collapse .navbar-collapse --> 
       </div><!-- .container --> 
     </nav><!-- #header-nav --> 
  </header> 
    <div id="call-btn" class="visible-xs"> 
     <a class="btn" href="tel:410-602-5008"> 
     <span class="glyphicon glyphicon-earphone"></span> 
     410-602-5008 
     </a> 
   </div> 
   <h2 id="menu-categories-title" class="text-center">Menu Categories</h2> 
 <div class="text-center"> 
   Substituting white rice with brown rice or fried rice after 3:00pm will be $1.50 for a pint and $2.50 for a quart. 
 </div>
   <div class="jumbotron"> 
      <img src="images/jumbotron_768.jpg" alt="Picture of restaurant" class="img-responsive visible-xs"> 
     </div> 
      <div id="home-tiles" class="row"> 
       <div class="col-md-4 col-sm-6 col-xs-12"> 
         <a href="#" onclick="$dc.loadMenuCategories();"><div id="menu-tile"><span>menu</span></div></a> 
       </div> 
       <div class="col-md-4 col-sm-6 col-xs-12"> 
         <a href="#" onclick="$dc.loadMenuItems({{randomCategoryShortName}});"> 
           <div id="specials-tile"><span>specials</span></div> 
         </a> 
       </div> 
       <div class="col-md-4 col-sm-12 col-xs-12"> 
         <a href="https://www.google.com/maps/place/David+Chu's+China+Bistro/@39.3635874,-76.7138622,17z/data=!4m6!1m3!3m2!1s0x89c81a14e7817803:0xab20a0e99daa17ea!2sDavid+Chu's+China+Bistro!3m1!1s0x89c81a14e7817803:0xab20a0e99daa17ea" target="_blank"> 
           <div id="map-tile"> 
             <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3084.675372390488!2d-76.71386218529199!3d39.3635874269356!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c81a14e7817803%3A0xab20a0e99daa17ea!2sDavid+Chu&#39;s+China+Bistro!5e0!3m2!1sen!2sus!4v1452824864156" width="100%" height="250" frameborder="0" style="border:0" allowfullscreen>
             </iframe> 
             <span>map</span> 
           </div> 
         </a> 
       </div> 
     </div><!-- End of #home-tiles --> 
      <div class="menu-item-tile col-md-6"> 
   <div class="row"> 
     <div class="col-sm-5"> 
       <div class="menu-item-photo"> 
         <div>{{short_name}}</div> 
         <img class="img-responsive" width="250" height="150" src="images/menu/{{catShortName}}/{{short_name}}.jpg" alt="Item"> 
       </div> 
       <div class="menu-item-price">{{price_small}}<span> {{small_portion_name}}</span> {{price_large}} <span>{{large_portion_name}}</span>
       </div> 
     </div> 
     <div class="menu-item-description col-sm-7"> 
       <h3 class="menu-item-title">{{name}}</h3> 
       <p class="menu-item-details">{{description}}</p> 
     </div> 
   </div> 
   <hr class="visible-xs"> 
 </div> 
   <div class="col-md-3 col-sm-4 col-xs-6 col-xxs-12"> 
   <a href="#" onclick="$dc.loadMenuItems('{{short_name}}');"> 
     <div class="category-tile"> 
       <img width="200" height="200" src="images/menu/{{short_name}}/{{short_name}}.jpg" alt="{{name}}"> 
       <span>{{name}}</span> 
     </div> 
   </a> 
 </div>
  <h2 id="menu-categories-title" class="text-center">{{name}} Menu</h2> 
 <div class="text-center">{{special_instructions}}</div> 
   <div id="xs-deliver" class="text-center visible-xs">* We Deliver</div> 
   <div id="main-content" class="container"></div> 
   <footer class="panel-footer"> 
     <div class="container"> 
       <div class="row"> 
         <section id="hours" class="col-sm-4"> 
           <span>Hours:</span><br> 
           Sun-Thurs: 11:15am - 10:00pm<br> 
           Fri: 11:15am - 2:30pm<br> 
           Saturday Closed 
           <hr class="visible-xs"> 
         </section> 
         <section id="address" class="col-sm-4"> 
           <span>Address:</span><br> 
           7105 Reisterstown Road<br> 
           Baltimore, MD 21215 
           <p>* Delivery area within 3-4 miles, with minimum order of $20 plus $3 charge for all deliveries.</p> 
           <hr class="visible-xs"> 
         </section> 
         <section id="testimonials" class="col-sm-4"> 
           <p>"The best Chinese restaurant I've been to! And that's saying a lot, since I've been to many!"</p> 
           <p>"Amazing food! Great service! Couldn't ask for more! I'll be back again and again!"</p> 
         </section> 
       </div> 
       <div class="text-center">&copy; Copyright David Chu's China Bistro 2016</div> 
     </div> 
   </footer> 
   <!-- jQuery (Bootstrap JS plugins depend on it) --> 
   <script src="js/jquery-2.1.4.min.js"></script> 
   <script src="js/bootstrap.min.js"></script> 
   <script src="js/ajax-utils.js"></script> 
   <script src="js/script.js"></script>
   <script src="js/npm.js"></script> 
 </body> 
</html> 
