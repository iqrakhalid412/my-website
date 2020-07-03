<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">
  <script src="https://code.jquery.com/jquery-3.4.1.slim.min.js" integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js" integrity="sha384-Q6E9RHvbIyZFJoft+2mJbHaEWldlvI9IOYy5n3zV9zzTtmI3UksdQRVvoxMfooAo" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
/* background image */

html{
  scroll-behavior: smooth;
}
.color{
  text-decoration:blue;
}
.contact{
  margin-top:50px;
}
#barbav{
    background-size:100% 100%;
    background-attachment: fixed;
 width:100%;
  height:950px;
}
body img
{
    width:100%;
    height:950px;
    background-size:100% 100%;
    background-attachment: fixed;
}
/* logo */
nav div img{
  
  
  width:150px;
  height:190px;
}
p{
  margin-top:50px;
}
#bg_color{
  background-color:#34d2eb ;
}

/* jumbotron */
 #jumb{
padding-top:120px;
padding-bottom:0px;
} 
 </style>
 <script>

   //employment
    function valid(){
            var us=document.getElementById("us").value;
            if(us==""){
                document.getElementById("usrname").innerHTML="*required user name";
                return(false);
            }
            if(us.length<=2 || user.length>=10){
                document.getElementById("usrname").innerHTML="*characters must be between 2 & 10";
                return(false);
            }
            if(!isNaN(us)){
                document.getElementById("usrname").innerHTML="*only characters required";
                return(false);
            }
         var phone=document.getElementById("ph").value;
        if(phone=="")
        {
          document.getElementById("phn").innerHTML="*required phone number";
          return(false);
        }
        if(phone.length<0 || phone.length>11){
          document.getElementById("phn").innerHTML="*invalid phone number";
          return(false);

        }
            var x=document.getElementById("eml").value;
            if(x==""){
                document.getElementById("em").innerHTML="*required email address";
                return (false);
            }
            if((x.indexOf('@')<1) || (x.lastIndexOf('.')>=x.length-2) || (x.lastIndexOf('.')-x.indexOf('@')<3)){
                document.getElementById("em").innerHTML="*invalid";
                return(false);
        }
        var prior=document.getElementById("prior").value;
        if(prior=="")
        {
          document.getElementById("pr").innerHTML="*required ";
          return(false);
        }
        var c=document.getElementById("cj").value;
        if(c=="")
        {
          document.getElementById("c_j").innerHTML="*required ";
          return(false);
        }
        var pm=document.getElementById("pm").value;
        if(pm=="")
        {
          document.getElementById("p_m").innerHTML="*required";
          return(false);
        }
        // var ava=document.forms.container;
        // for(var i=0;i<ava.length;i++){
        //     if(ava[i].checked==true){
        //  return(true);
        //  }}
         var a=document.getElementById('t').checked;
         var b=document.getElementById('th').checked;
         var c=document.getElementById('f').checked;
         var d=document.getElementById('fr').checked;
         var e=document.getElementById('s').checked;
         var f=document.getElementById('sa').checked;
         if((a==" ") &&(b==" ") &&(c==" ") && (d==" ") &&(e==" ") &&(f==" ")){
          document.getElementById("avi").innerHTML="*required";
         return(false);
        }
        var any=document.getElementById("any").value;
        if(any=="")
        {
          document.getElementById("an").innerHTML="* required";
          return(false);
        }

  }

//navbar
 function w(){
   var x=document.getElementById("w");
   x.style.color="gray";
 }
 function men(){
   var x=document.getElementById("men");
   x.style.color="gray";
  
 }
 function b(){
   var x=document.getElementById("b");
   x.style.color="gray";
 }
 function re(){
   var x=document.getElementById("re");
   x.style.color="gray";
 }
 function ct(){
   var x=document.getElementById("ct");
   x.style.color="gray";
 }

 function em(){
   var x=document.getElementById("em");
   x.style.color="gray";
 }


//contact
     // for user
function validation(){
        var user=document.getElementById("user").value;
        if(user===""){
            document.getElementById("username").innerHTML="*Name is required";
            return(false);
        }
        if((user.length<=2) || (user.length>=20))
        {
            document.getElementById("username").innerHTML="*user length must be between 2 and 20";
            return false;
        }
        if(!isNaN(user)){
            document.getElementById("username").innerHTML="*only characters are allowed";
            return false;}
    //for email
        var email=document.getElementById("email").value;
        if(email===""){
            document.getElementById("e").innerHTML="*Email is required";
            return false;
        }

        if((email.indexOf("@")<1) || (email.lastIndexOf(".")>=email.length-2) || (email.lastIndexOf(".")-email.indexOf("@")<3))
        {
            document.getElementById("e").innerHTML="*invalid";
            return false;
        }
    //subject
        var subject=document.getElementById("subject").value;
        if(subject==""){
            document.getElementById("subj").innerHTML="*Subject is required";
            return false;
            }
     //message
        var message=document.getElementById("message").value;
        if(message==""){
            document.getElementById("me").innerHTML="*Message is required";
            return false;
        }       
}



// onblur
function blur(){
  var x=document.getElementById("user");
  x.style.color="red";
}




 </script>
</head>
<body>

      <!--<div class="container-fluid">-->
      <div>
    <nav class="navbar navbar-expand-md navbar-light show on scroll fixed-top " id="bg_color" >
  <div class="mt-2 ml-2">
    <img src="logo.png" >
  </div>
  
    <a class="navbar-brand ml-4 mt-5 "  style="color: white;" id="w" onclick="w()"  href="#wel">WELCOME</a>
   
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
   
    <div class="collapse navbar-collapse" id="navbarNav">
     
      <ul class="navbar-nav">
        <li class="nav-item">
          <a class="navbar-brand mt-5 color" style="color: white;" id="men" onclick="men()" href="#m" >MENU</a>
          <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          -->
         <!-- <a class="nav-link" href="#">Reservations</a> -->
        </li>
        <li class="nav-item " >
          <a class="navbar-brand mt-5 color" style="color: white;" id="b" onclick="b()" href="#barb">BAR & BAVERAGES</a>
          <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button> -->
         
          <!-- <a class="nav-link" href="#" id="n">Bar $Bevrages <span class="sr-only">(current)</span></a> -->
        </li>
        <li class="nav-item">
          <a class="navbar-brand mt-5 "style="color: white;" id="re" onclick="re()" href="#r" >RESERVATIONS</a>
          <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button> -->
         
          <!-- <a class="nav-link" href="#">Reservations</a> -->
        </li>
        <li class="nav-item">
          <a class="navbar-brand mt-5 " style="color: white;" id="ct" onclick="ct()"href="#c" >CONTACT US</a>
          <!-- <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button> -->
          
          <!-- <a class="nav-link" href="#">Contact</a> -->
        </li>
        <!-- <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>-->
        <li class="nav-item active" >
          <a class="navbar-brand mt-5 " style="color: white;" id="em" onclick="em()" href="#empl">EMPLOYMENT</a>
      </li>
      </ul>
     
    </div>
    
  </nav>
<div id="wel">
   <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1537312713591-LYL2B29NQ5V5ZLCXS0YU/ke17ZwdGBToddI8pDm48kK60W-ob1oA2Fm-j4E_9NQB7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0kD6Ec8Uq9YczfrzwR7e2Mh5VMMOxnTbph8FXiclivDQnof69TlCeE0rAhj6HUpXkw/IMG_7392.JPG?format=1500w">
</div>
      </div>










<!-- Menu -->









<div class="text-secondary"id="m">
      <!-- <div style="margin-top:150px"> -->
        <img src=menu.jpg>
        <!-- </div> -->
        <section>
      
          <div class="container text-secondary">
      
            <div class="row">
      
              <div class="col-lg-9 col-md-9 col-sm-9  text-center text-info" style="padding-top: 80px;">
                     <h5 style="letter-spacing: 3px;">
                       Life is celebration.Enjoy it well.<br>
                      
                     <h5>
                      <h6>-Uruj Shahid</h6>
              </div>
      
              <div class="col-lg-3 col-md-3 col-sm-3 mt-5 pt-5">
                <h6 >
                  <b>Location</b>
                </h6>
              
            
                512 East 9th Street
                <br> 
      
               Lawrence, Kansas 66044
          
              
      
      
               </div>
            </div>
      
            <div class="row">
      
            
              <div class="col-lg-9 col-md-9 col-sm-9">
      
              
                     <p>
                      Culinaria is a cozy restaurant in East Lawrence with a (sometimes) lively atmosphere.
                       Located in one of Lawrence’s most historic buildings, Culinaria opened in 2009 as a customized catering company and private event space.
                        After 8 years in the event’s industry, husband-and-wife owners, Aaron and Regan Pillar, decided to open a weekend restaurant, 
                        featuring foods they love,inspired by the spices and culinary aesthetic of the Mediterranean. 
                        Now open every Thursday, Friday and Saturday evening, Culinaria serves Mediterranean-inspired dinner selections,
                         homemade sweets and fresh fruit cocktails along with wine pairings and craft beer. 
                        With flavorful, innovative food and a warm, friendly environment, the folks at Culinaria invite you to come in, relax and celebrate 
                      one of life’s greatest joys … the simple pleasure of eating and drinking.  
                     </p>
                     
              </div>
             <div class="col-lg-3 col-md-3 col-sm-3 mt-5">
              <h6>
                <b>
                Phone</b>
              </h6>
              785.766.8591
            <br>
            <br>
            <br> 
            <h6> <b>Email </b></h6>
      
              sayhi@culinariafoodandwine
              <br>
              .com
             
               
                 
               </div>
              
            </div>
            
            <div class="row" >
              <div class="col-lg-9 col-md-9 col-sm-9 mt-5 mb-5">
              
           <h6><b>
            Hours:</b>
           </h6>
           <br>
           <h6 >
             <b>
            Thursday | Friday | Saturday                 3:30p-9p
            </b>
            </h6>
          </div>
            </div>
           
              <div class="row mt-5 mb-5">
            
                <div class="col-lg-6 col-md-6 col-sm-6 ">
                  <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1537314666072-NTTS4JNRAQ265O4Y8WA8/ke17ZwdGBToddI8pDm48kNLQu-B0RRAfDtkSaNKjdh97gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z5QPOohDIaIeljMHgDF5CVlOqpeNLcJ80NK65_fV7S1Ucrtycac1QImJ63llVaF2ZqExZUeFLe6NVW50JARQ002A_BAmoM8KfSaR3f6p1HyQw/IMG_2142+2.jpg" style="height:350px">
                </div>
          <div class="col-lg-6 col-md-6 col-sm-6 text-info">
            <p>
            
             <span class="display-4">
               Our building
             </span>
             <br>
             <br>
              
            
              Located on the northwest corner of 9th and New Jersey, 
             the building housing Culinaria was originally constructed for the Kansas
              Cavalry after Quantrill’s raid (The Lawrence Massacre) in the fall of 1863.
               As a barn and carriage house, the dining room was used as a horse stable with 
               a hay loft overhead. The space was also a butcher’s shop and slaughter house in
                the 1950’s as well as a Volkswagen mechanic in the 1970’s and 80’s.
            </p>
      
          </div>
          </div>
        </div>
        <div class="text-center text-capitalize text-secondary" style="letter-spacing: 1px;">
         <p> Happy Hour Dinner</p> 
       
        <p>
        Thursday-Saturday 3:30 pm - 9 pm</p>
        <h4 class="text-info" style="letter-spacing: 1px; padding-bottom: 20px;"> $6 MEZZE SMALL PLATES! </h4>
      </div>
      <div class="container text-secondary  mb-5">
      <div class="row">
        <div class="col-lg-6 col-md-6 col-sm-6">
          <h5>Spicy Hummus & Falafel<span style="padding-left:150px;">$6</span></h5>
          
          Hummus Tehina with Schug, served with Falafel, Flatbread & Pickles
      
          <br>
          <br>
          
          <h5>Fried Artichoke Hearts <span style="padding-left:162px;">$6</span></h5>
          with Jalapeño-Caper Relish
          
        
        <br>
        <br>
          <h5> Jerusalem Hummus <span style="padding-left:185px;" >$6</span></h5>
          Our Hummus topped with Spiced Beef, Za’tar Flatbread
          <br><br><br>
        
        </div>
      
        
        <div class="col-lg-6 col-md-6 col-sm-6">
          <h5>Crispy Smashed Potato<span style="padding-left:160px;">$6</span>
          </h5>
          
          Whole Baked Potato, Smashed & Fried, Drizzled with Anchovy Vinaigrette, Shaved Parmesan, Scallions
      
          <br>
          <br>
          <br>
         <h5> Squash & Chorizo<span style="padding-left:210px;" >$6</span>
        </h5>
        
         
         
          Pan-roasted Squash, Spanish Chorizo, Goat Cheese, Pomegranate Molasses
          
          <br>
          <br>
      
         <h5> Fried Cauliflower with Labneh<span style="padding-left:100px;" >$6</span>  </h5>
        
          with House Spice, Pickled Red Onions
      </div>
        
      </div>
      </div>
      <!-- bar -->
      
      
      <div class="container text-secondary mt-5 mb-5">
        <h4 class="text-center text-capitalize text-info" style="letter-spacing: 1px; padding-bottom: 30px;">Bar</h4>
      <div class="row">
        <div class="col-lg-6 col-md-6 col-sm-6">
          <h5> Honey Buck<span style="padding-left:255px;">$6</span></h5>
          
          
      
          <br>
        
          
          <h5> Grapefruit-Ginger Gin Fizz<span style="padding-left:130px;">$6</span></h5>
          
        
        
        <br>
          <h5> Prickly Pear Tequila Rickey<span style="padding-left:125px;" >$6</span></h5>
          
          <br>
          <h5>Fall Rum Punch<span style="padding-left:225px;">$6</span>
        </div>
      
        <br>
        <div class="col-lg-6 col-md-6 col-sm-6">
          <h5>Horsefeather<span style="padding-left:245px;">$6</span>
          </h5>
          
          <br>
          
          <br>
         <h5> Sangria<span style="padding-left:300px;" >$7</span>
        </h5>
        
         
        Red Wine, Cointreau, Citrus, Berries, Seasonal Fruit
          
          
          <br>
          <br>
      
         <h5> Wine<span style="padding-left:320px;" >$2 off</span>  </h5>
        
          By the glass
        
        </div>
        
      </div>
      
      </div>
      <h3 class="text-info text-capitalize text-center " style="padding-bottom: 60px;" >PLUS, SPECIAL FEATURES EACH WEEKEND!<h3>
      
      </div>
          
        </section>
    </div>



















<!-- bar and baverages -->









<div class="text-secondary"id="barb">

  <img src="bar.jpg" id="barbav">  
      <div class="pt-5" style="background-color:#34d2eb;"> 
      <div class="container">
        <div class="row">
          <div class="col-lg-6 col-md-6 col-sm-6">
        <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1533074850113-29A6VIYPK66931F0NV86/ke17ZwdGBToddI8pDm48kDk1dm1oSR9gCa1mX4KqzjN7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0luj0xCD0oh5KMc0gpox0u-wQWxfQHg04OxgQwaUq2yiAcNt5Kg2tE9yEtYfM4xwaw/david-becker-677440-unsplash.jpg" class="d-inline" id="image" style="height:300px">
        
        
          </div>
        
         <div class="col-lg-6 col-md-6 col-sm-6 px-5 py-5" style="background-color:white">
           <div class=" text-info" style="letter-spacing:1px;" > 
          
            <h5>Bubbles & White Wine</h5>
            Catalonia, Spain | Torre Oria Brut Cava $8 |<br>
             $32<br>
            
            Mendocino, California | Bliss Rose $8 | $32<br><br>
            
            Rioja, Spain | Cune Monopole Blanco $36<br><br>
            
            Veneto, Italy | Tre Fili Pinot Grigio $9 | $32<br><br>
            
            Bordeaux, France | Clos des Lunes Bordeaux <br>
            Blanc $50<br><br>
            
            Macedonia, Greece | 14|27 >Amazia Organic <br>
            $10 | $40<br><br>
            
            New Zealand | Koha Sauvignon Blanc $9<br>
             | $32<br><br>
            
            Mendocino, California | Brutocao Chardonnay<br>
             $11 |$40<br><br>
            
            Columbia Valley, Washington| Dunham<br>
             Cellars $60
          
  
         </div>
         </div>
          </div>
      </div></div>
      <div class="pt-5" style="background-color:#34d2eb;"> 
        <div class="container">
          <div class="row">
            <div class="col-lg-6 col-md-6 col-sm-6">
              <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1533074891341-4K55CDDK89X0BK9K5L4D/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/jehyun-sung-477890-unsplash.jpg?format=500w" class="d-inline" id="image" style="height:300px">
        
          
            </div>
          
           <div class="col-lg-6 col-md-6 col-sm-6 d- px-5 py-5" style="background-color:white">
             <div class=" text-info" style="letter-spacing:1px;" > 
             <h3> Red Wine</h3>
              Oregon | Cooper Hill Pinot Noir $11 | $44<br><br>
              
              Central Coast, California | Wonderwall Pinot<br>
               Noir $55<br><br>
              
              Côtes du Rhône, France | Barville Côtes du <br>
              Rhône $40<br><br>
              
              Portugal | Cabriz Red Blend $8 | $32<br><br>
              
              Macedonia, Greece | 14|27 Xino Organic $10<br>
               | $40<br><br>
              
              Rioja, Spain | Cerro Añon Tempranillo $12 |<br>
               $44<br><br>
              
              Rioja, Spain | Viña Alberdi Reserva Tempranillo <br>
              $50<br><br>
              
              Chile | Casas del Bosque Cabernet $12 | $44 <br>
              Gran Reserva
              
  
  
  
  
  
  
    
           </div>
           </div>
            </div>
            
    </div>
    </div>
    <div class="pt-5" style="background-color:#34d2eb;"> 
      <div class="container">
        <div class="row">
          <div class="col-lg-6 col-md-6 col-sm-6">
        <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1504379020466-Q28AMGOS4SE5XF5QOO8A/ke17ZwdGBToddI8pDm48kDHPSfPanjkWqhH6pl6g5ph7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0mwONMR1ELp49Lyc52iWr5dNb1QJw9casjKdtTg1_-y4jz4ptJBmI9gQmbjSQnNGng/frank-luca-71973.jpg?format=500w" class="d-inline" id="image" style="height:300px">
        
        
          </div>
        
         <div class="col-lg-6 col-md-6 col-sm-6 d- px-5 py-5" style="background-color:white">
           <div class=" text-info" style="letter-spacing:1px;" > 
            <h3>Beer</h3>
            Life Coach Lager (Washington, KS) $3.50<br><br>
            
            Defiance Kansan American Wheat (Hays, KS)<br>
             $4.00<br><br>
            
            New Belgium DayBlazer Easy Going Ale (CO)<br>
             $4.00<br><br>
            
            Dogfish Head SeaQuench Ale (DE) $5.00<br><br>
            
            O’dell Drumroll APA (CO) $4.00<br><br>
            
            Yankee Tank Red Dirt Country Ale $4.00 <br>
            (Lawrence, KS)<br><br>
            
            Free State Copperhead Pale Ale $4.00 <br>
            (Lawrence, KS)<br><br>
            
            Tropic Plunder (CA) $4.75<br><br>
            
            Deschute’s Fresh-squeezed IPA (OR) $4.50<br><br>
            
            Left Hand Brewing Co Milk Stout (CO) $4.50
            
         </div>
         </div>
          </div>
      </div></div>
      <div class="pt-5" style="background-color:#34d2eb;"> 
        <div class="container">
          <div class="row">
            <div class="col-lg-6 col-md-6 col-sm-6">
          <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1533075743098-MOANGSKA4C6CYZ7C8UQS/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/chinh-le-duc-460165-unsplash.jpg?format=500w" class="d-inline" id="image" style="height:300px">
          
          
            </div>
          
           <div class="col-lg-6 col-md-6 col-sm-6 d- px-5 py-5" style="background-color:white">
             <div class=" text-info" style="letter-spacing:1px;" > 
            
              <h3>Spirits</h3>
              Vodka: Titos (Austin, TX) $5.50 | Reyka <br>
              (Iceland) $6.00<br><br>
              
              Gin: Sloan's Dry (Netherlands) $6.00 |<br>
               Principle de los Apostoles Yerba Matte 
               <br>(Argentina) $6.50<br><br>
              
              Whiskey (Rye | Bourbon): Old Overholt Rye <br>
              $5.50 | Bulleit $6.50<br><br>
              
              Tequila: Espolon (Mexico) $5.00 | Demetrio <br>
              Reposado (Mexico) $5.50<br><br>
              
              Scotch: Glenlivet $10.00
              <br><br>
              
              Classic Cocktails: Martinis | Manhattans | <br>
              Margaritas | Highballs
  
  
  
  
  
  
  
           </div>
           </div>
            </div>
        </div></div>
        <div class="pt-5" style="background-color:#34d2eb;"> 
          <div class="container">
            <div class="row">
              <div class="col-lg-6 col-md-6 col-sm-6">
            <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1537397946593-5CBY45OPB9R37DX9LN05/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/freestocks-org-626892-unsplash.jpg?format=500w" class="d-inline" id="image" style="height:300px">
            
            
              </div>
            
             <div class="col-lg-6 col-md-6 col-sm-6 d- px-5 py-5" style="background-color:white">
               <div class=" text-info" style="letter-spacing:1px;" > 
              
  
                <h3>Culinaria Cocktails<br>
                $8.50</h3>
                — $6 during Happy Hour —
                
                Honey Buck<br><br>
                
                Grapefruit-Ginger Gin Fizz<br><br>
                
                Prickly Pear Tequila Rickey<br><br>
                
                Fall Rum Punch<br><br>
                
                Horsefeather<br><br>
                
                Sangria (Red Wine, Cointreau, Citrus, Berries,<br>
                 Seasonal Fruit) $7 | $5.50 Happy Hour!
  
  
  
  
  
              
      
             </div>
             </div>
              </div>
          </div></div>
          <div class="pt-5 pb-5" style="background-color:#34d2eb;"> 
            <div class="container">
              <div class="row">
                <div class="col-lg-6 col-md-6 col-sm-6">
              <img src="https://images.squarespace-cdn.com/content/v1/5998924249fc2bee42db01ab/1537398065230-4OSOR5S3YV6NFMXPIN78/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/nick-fewings-633894-unsplash.jpg?format=500w" class="d-inline" id="image" style="height:300px">
              
              
                </div>
              
               <div class="col-lg-6 col-md-6 col-sm-6 d- px-5 py-5" style="background-color:white">
                 <div class=" text-info" style="letter-spacing:1px;" > 
                
      <h3>Fancy Drinks</h3>
                  Happy Drink (Reyka, Lambic Framboise,<br>
                   Fresh-squeezed Lemonade) $10.00<br><br>
                  
                  Pomegranate Moscow Mule (Reyka, Fresh<br>
                   Lime, Ginger Beer, Pomegranate San<br>
                    Pellegrino | Served in a Copper Mug) $10.00<br><br>
                  
                  Cherry Rickey (Reyka, Luxardo Cherry Syrup,<br>
                   Fresh Lime, Soda) $10.00<br><br>
                
                  
                  Vodka Martini (Tom’s Town Vodka, Vermouth,<br>
                   splash of Olive Juice, Olive, Up) $11.50<br><br>
                  
                  Park Slope Cosmopolitan (Reyka, Fresh Lime,<br>
                   Grapefruit-Ginger, Up) $11.50<br><br>
                  
                  Blood Orange Sling (Apostoles Gin, Blood <br>
                  Orange San Pellegrino, Bitters) $10.00<br><br>
                  
                  Gin Martini (Tom’s Town Gin, Vermouth, splash <br>
                  of Olive Juice, Olive, Up) $11.50<br><br>
                  
                  Margarita (Cimarron Blanco, Fresh-squeezed<br>
                   Sour, Lime) $9.50<br><br>
                  
                  Fancy Tequila (Demetrio Reposado, Fresh<br>
                   Orange, Cherry, Lime) $10.00<br><br>
                  
                  Sangria (Red Table Wine, Cointreau, Berries,<br>
                   Citrus) $7.00<br><br>
                  
                  Basil Cranberry Julep (Xicaru Mezcal, 1883<br>
                   Cranberry Basil, Fresh Lime, Soda) $9.50<br><br>
                  
                  Cherry Daiquiri (Real McCoy Rum, Fresh Lime,
                  <br> Luxardo Cherry Syrup) $9.50<br><br>
                  
                  Rooster Tail (Avuá Amburna, Cinzano Sweet<br>
                   Vermouth, Regan’s Orange Bitters) $12.00<br><br>
                  
                  Spiced Pear Rye (Old Overholt Rye, Spiced <Br>
                    Pear Simple Syrup, Lemon, Soda, <br>
                    > Pepper) $8.50<Br><br>
                  
                  Manhattan (Bulleit Bourbon, Cinzano Sweet<br>
                   Vermouth, Bitters, Cherry) $11.50<br><br>
                  
                  Apple Old Fashioned (Ch Bourbon, Orange<br>
                   Bitters, Cherry, Orange Wedge, Apple Cider<br>
                    Ice Cube) $12.00
  
  
  
        
               </div>
               </div>
                </div>
            </div></div>
            
  
  
  
        </div>
  
  
  
          
      
    




<!-- reservatin -->


  <div  id="r">
 
    <img src="re.jpg">
    <div class="container-fluid py-5 bg-secondary">
    <h1 class="text-center pt-4">Make a Reservation</h1>
   <div class="text-center"> <button type="Submit" class="btn btn-primary "> Find A Table</button><br>
   <br class="text-primary">
    Having difficulties making a reservation?
  <br>
    We can help.
    <br>
    Please call or text your request to (785) 766-8591, and we'll likely find you a spot.</div>
    </div>
  
   
  </div>
    
    
      </div>
    
      </div>
    













<!-- contact -->







<div class="contact text-secondary" id="c">
  <div class="container text-secondary" >
      <form onsubmit="return validation()">
        <div class="form-row">
              <div class="form-group col-md-6 pt-3">
             <!-- name -->
             <label>Name*</label>
             <input type="text" name="FirsstName" class="form-control" onblur="blur()"id="user">
                  <label>FirstName</label>
                  <div> <span id="username" class="text-light bg-danger"></span></div></div>

              <div class=  "form-group col-md-6 pt-5">

                  <input type="text" name="LastName" class="form-control" id="user">
                  <label>LastName</label>
                </div>
                </div>
           
         
        
      <!-- email -->
               <div class="form-group">
                <label>Email*</label>
                   <input type="text" name="email" class="form-control"  id="email" > </div>
     <div>
         <span id="e" class="text-light bg-danger"></span>

     </div>
              

     <!-- subject -->
            <div class="form-group">
                <label>Subject*</label>
                <input type="text" name="Subject" class="form-control" id="subject"> </div>
                
                <div> 
                    <span id="subj" class="text-light bg-danger"></span>
                </div>



   <!-- message -->

       <div class="form-group">
           <label>Message*</label><br>
           <small>For catering inquiries, please provide the date, time, guest count and location of your event, and we'll respond with a potential menu and estimate!</small>
           <textarea class="form-control " rows="5" id="message"></textarea>
       </div>
       <div>
           <span id="me" class="text-light bg-danger"></span>
       </div>

       <!-- submit -->
       <div>
           <input type="submit" value="Submit" class="btn btn-outline-secondary p-2">

       </div>

      </form>

  </div>
    </div>

   




<!-- employee -->

<div class="text-secondary mb-5"id="empl">
      <div class="e">
        <div class="container text-center mt-5 text-info">
            <h1>Application</h1>
           </div>
        <div class="container">
            <form name="forms" onsubmit="return valid()">
              <div class="form-row">
                <div class="form-group col-md-6 pt-3">
                  <!-- name -->
                  <label>Name*</label>
                  <input type="text" name="name" class="form-control" id="us">
                  <label>FirstName</label></div>


                  <div class="form-group col-md-6 pt-5">
                      <input type="text" name="name" class="form-control">
                      <label>LastName</label></div>
                
                    
                    <div>
                    <span id="usrname" class="text-white bg-danger"></span></div>
                     </div>
              <!-- phone# -->
                <div class="form-row">
              <div class="form-group col-md-3 pt-3">
                   <label >Phone*</label> 
              <input type="phone number" class="form-control"id="ph">
              </div>

                </div>
              <div><span id="phn" class="text-light bg-danger"></span></div>
                <!-- email -->
              <div class="form-group">
                <label>Email</label>
                <input type="text" name="email" class="form-control" id="eml"> </div>
                <div><span id="em" class="text-light bg-danger"></span>
                </div>



               <div class="form-group">
                <label>Prior Service Experience</label><br>
                <small>Restaurant or Events/Catering </small>
                <br>
                <textarea class="form-control" id="prior" rows="5"></textarea>
              
              </div>
              <div><span id="pr" class="text-light bg-danger"></span>
              </div>

              <div class="form-group">
                <label>Current Job*</label><br>
                <small> Please include hire date and current position </small>
                <br>
                <textarea class="form-control" id="cj" rows="5"></textarea>
              
              </div>
              <div><span id="c_j" class="text-light bg-danger"></span>
              </div>
              <div class="form-group">
                <label for="exampleFormControlTextarea1">Prior Employment*</label><br>
                <small> Please include your dates of employment, position, and reason for leaving
                </small>
                <br>
                <textarea class="form-control" id="pm" rows="5"></textarea>
              </div>
              <div><span id="p_m" class="text-light bg-danger"></span>
              </div>

              <label >Availability*</label> 
              <div >
              <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="t" >
                <label class="form-check-label" >
                    Thursday, 3 pm - 9:30 pm
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="th"  >
                <label class="form-check-label" >
                    Thursday, 5:30 pm - 10:30 pm
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="f" >
                <label class="form-check-label">
                    Friday, 3 pm - 10 pm
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="fr" >
                <label class="form-check-label" >
                    Friday, 5:30 pm - 11 pm
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="s"  >
                <label class="form-check-label" >
                    Saturday, 3 pm - 10 pm
                </label>
            </div>
            <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="sa" >
                <label class="form-check-label" >
                    Saturday, 5:30 pm - 11 pm
                </label>
            </div>
          
               <div><span id="avi" class="text-danger"></p></div>
            
             <div class="form-group">
                <label>Anything else you'd like us to know! </label><br>
                <textarea class="form-control"  id="any" rows="5"></textarea>
              
              </div>
              <div><span id="an" class="text-light bg-danger"></span></div>
              
            
 

                <!-- <div class="form-group col-md-6">
                  <label for="inputCity">City</label>
                  <input type="text" class="form-control" id="inputCity">
                </div>
                <div class="form-group col-md-4">
                  <label for="inputState">State</label>
                  <select id="inputState" class="form-control">
                    <option selected>Choose...</option>
                    <option>...</option>
                  </select>
                </div>
                <div class="form-group col-md-2">
                  <label for="inputZip">Zip</label>
                  <input type="text" class="form-control" id="inputZip">
                </div>
              
              <div class="form-group">
                <div class="form-check">
                  <input class="form-check-input" type="checkbox" id="gridCheck">
                  <label class="form-check-label" for="gridCheck">
                    Check me out
                  </label>
                </div>
              </div>  -->
              <button type="submit" class="btn btn-secondary px-4">Submit</button>
            </form>
          </div>
      </div>
</div>
</div>
        </div>
</div >
<div class="jumbotron jumbotron-fluid mt-5 bg-info" id="jumb">
  <i class="fa fa-facebook-f fa-2x"></i>
  <div class="container-fluid text-center text-secondary " id="cont" style="background-color: black; padding-bottom:120px;">
    <div style="padding-top:70px">Powered by Squarespace</div>

    
  </div>
</div>

<!-- <div class="jumbotron jumbotron-fluid bg-dark">
</div> -->

<!-- <i class="fa fa-facebook-square fa-3x"></i> -->

      </body>
      </html>


 



