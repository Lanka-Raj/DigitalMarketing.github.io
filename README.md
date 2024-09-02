# DigitalMarketing.github.io
## Personal
### Order
#### Marketing
<!DOCTYPE html>
<html>

<head>
    <link rel="stylesheet" type="text/css" href="style.css" />
</head>

<body>
<div id="container">
    <header>
    <img src="/res/d7cbda8e-912d-4be0-86fd-b0177da8c57b/6125150314089790437-removebg-preview.png" id="logoImg"/>
        <h4 id="brandingName">Druk Arts </h4>
    <ul>
       <li id="nav-home">HOME</li> 
         <li id="nav-about">ABOUT</li> 
        
        
        </ul>
    </header>
    
<!-- homepage     -->
    <div id="home">
    <h1>Druk Arts And Crafts Gallery</h1>
        <img id="clothImg" src="/res/d7cbda8e-912d-4be0-86fd-b0177da8c57b/What-is-Bhutan-Famous-For.jpg" />
    
    </div>
<!--about page      -->
    <div id="about">
    <h1>About Us</h1>
        <div class="card">
        <div class="card-inner">
            <div class="front">
            <img id="img" src="/res/d7cbda8e-912d-4be0-86fd-b0177da8c57b/a-z-about-reading-2.jpg" />
            </div>
            <div class ="back">
            <h3>Tashi Wangchk</h3>
               
                <h2>CEO</h2>
               
            </div>
            
            </div>
        
        
        </div>
    </div>
    
    </div>
    
    <script type="text/javascript" src="script.js"></script>
</body>

</html>


header {
  width: 600px;
  height: 80px;
  background-color: lemonchiffon;
  border-radius: 10px;
  box-shadow: 0px 5px 5px grey;
  display: flex;
  position: fixed;
  top:0;
  left: 0;
  z-index: 1;
}
#logoImg{
    width: 80px;
    height: 80px;
}
#brandingName{
    margin: 30px 5px;
    font-size: 18px;
}

ul li {
   list-style-type: none;
   display: inline-block;
   position: relative;
    left: 20%;
    margin: 15px 5px;
    font-size: 20px;
    font-weight: bolder;
    text-shadow: 2px 2px pink;
 }
ul li:hover{
    color: #0000ff;
     text-shadow: 2px 2px white;
    cursor: pointer;
}
#home{
    margin-top:100px;
    text-align: center;
}
#clothImg{
    width: 400px;
    box-shadow: 0px 3px 8px black;
    border-radius: 10px;
    
}
#clothImg:hover{
    transform: scale(1.1);
    transition-duration: 2s;
    cursor: pointer;
}
#about{
    max-width: 950px;
    margin: 0 auto;
    text-align: center;
    
}
#photo{
    width: 400px;
    box-shadow: 0px 3px 8px black;
    border-radius: 10px;
}
/* .front:hover{
     transform: scale(1.1);
    transition-duration: 1s;
    cursor: pointer;
} */
img {
    width: 300px;
    border-radius: 10px;
}

.card {
    display: inline-block;
    background-color: transparent;
    width: 220px;
    height: 170px;
    perspective: 1000px;
    margin: 5px;
    cursor: pointer;
     transform: scale(1);
    transition: 0.3s transform ease-out;
    transition: 0.3s transform ease-out;  
}

.card:hover {
    transform: scale(1.090);
}

 .card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    text-align: center;
    transition: transform 0.6s;
    transform-style: preserve-3d;
    border-radius: 5px;
    box-shadow: 0 4px 4px 0 rgba(0,0,0,0.3);
} 

.card.open .card-inner {
    transform: rotateY(180deg);  
}

.front, .back {
	position: absolute;
    width: 100%;
    height: 100%;
    box-sizing: border-box;
 	backface-visibility: hidden;
	backface-visibility: hidden;  
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;  
}

.front {
    background-size: cover;
    background-color: darksalmon;
    color: white;
    background-position: center;
}

.back {
	transform: rotateY(180deg);
    background-color: mintcream;
    padding: 20px;
}

.card h3 {
/*     background-color: rgba(0,0,0, 0.7); */
    padding: 15px;
    width: 100%;
}
#img{
    width: 400px;
    box-shadow: 0px 3px 8px black;
    border-radius: 10px;
}


var cards = document.querySelectorAll(".card");

cards.forEach(function(card) {
    card.addEventListener("click", function() {
        if (card.classList.contains("open")) {
            card.className = "card";
        }
        else {
            card.className = "card open";
        }
    });
});





 
