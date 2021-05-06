# Lipstick-shade-animation-with-css
.....html....
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <script src="script.js"></script>
    <html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" type="text/css" href="lipstick.css">
	<title>Lipstick Shades prototype</title>
</head>
<body>
  <div class="head"> 
  <h3><b>Lipstick Shades</b></h3>
  <h2>Keep calm and gloss on</h2>
    </div>
	<div class="lipsticks">
	<div class="one">
     <div class="tip"></div>
     <div class="middle"></div>
     <div class="base"></div>
      </div>
      <div class="two">
       <div class="tip2"></div>
     <div class="middle2"></div>
     <div class="base2"></div>
     </div>
      <div class="three">
       <div class="tip3"></div>
     <div class="middle3"></div>
     <div class="base3"></div>
     </div>
      <div class="four">
       <div class="tip4"></div>
     <div class="middle4"></div>
     <div class="base4"></div>
     </div>
     <div class="five">
       <div class="tip5"></div>
     <div class="middle5"></div>
     <div class="base5"></div>
     </div>
     <div class="six">
       <div class="tip6"></div>
     <div class="middle6"></div>
     <div class="base6"></div>
     </div>



</div>
  <!-- Confetti JS -->
  <script src="https://cdn.jsdelivr.net/gh/mathusummut/confetti.js/confetti.min.js"></script><script>confetti.start()</script>
</body>
</html>
  </body>
</html>
.....css......
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&display=swap');

body{
  background-image: url('https://www.gettyimages.in/detail/photo/portrait-of-a-nice-looking-woman-royalty-free-image/839310892');
  background-color: blueviolet;
  background-repeat: no-repeat;
  background-size: cover;
	display: flex;
	align-items: center;
	justify-content: center;
}
h3{
  animation: head 3s ease-in;
  position: absolute;
  top: -20px;
  left: 500px;
  font-size: 50px;
  font-family: 'Dancing Script', cursive;
  color: white;
}
@keyframes head{
  0%{ left: 25px; color: red;}
  25%{color: fuchsia;}
  50%{color: brown;}
  75%{color: magenta;}
  100%{color: peach;}
}
h2{
  animation: title 3s ease-in;
  position: absolute;
   bottom: -30px;
  left: 350px;
  font-size:55px;
  font-family: 'Dancing Script', cursive;
  color: gold;
}
@keyframes title{
  0%{left: 50px;}
  25%{}
  50%{}
  100%{}
}


.lipsticks{
	display: flex;
	margin: 5em auto;
	flex-direction: row;
}
.one, .two, .three, .four, .five, .six{
	padding-right: 10px;
}

.tip, .tip2, .tip3, .tip4, .tip5, .tip6{
	position: relative;
	height: 130px;
	width: 50px;
	box-shadow: inset 3px -5px 11px rgba(0,0,0,0.2);
	border-radius: 0px 20px 0px 0px;
	border-top-left-radius: 100px 140px;
	border-top-right-radius: 50px 140px;
	clip-path: polygon(0% 0%, 0% 100%, 100% 100%, 100% 50%, 50% 0%);
	animation-name: tip;
	animation-duration: 5s;
	animation-iteration-count: once;
}
@keyframes tip {
	0%{ height: 0px; }
	25%{ height: 35px; }
	50%{ height: 70px; }
	75%{ height: 100px; }
	100%{ height: 130px; }

}
.tip{
	background-image: radial-gradient(#c40233, #c40233, #c40233);
}
.middle, .middle2, .middle3, .middle4, .middle5, .middle6{
	position: relative;
	height: 105px;
	width: 70px;
	background-image: linear-gradient(silver, gray, silver);
    box-shadow: rgba(0,0,0,0.4);
	left: -10px;
	border-radius: 5px 5px 0px 0px ;

}
.base, .base2, .base3, .base4, .base5, .base6{
	position: relative;
	height: 150px;
	width: 80px;
	background-image: linear-gradient(black, black, black, black);
	left: -15px;
	box-shadow: 0px 3px 3px rgba(0,0,0,0.5);
  border-radius: 2px 2px 5px 5px;
}
.base:before{
	content: 'Red';
	position: relative;
	color: #f1fcfe;
	color: #f1fcfe;
	font-family: 'Dancing Script', cursive;
	font-size: 20px;
	bottom: -50px;
	right: -25px;
}
 .tip2{
	background-image: linear-gradient(#ff63c9, #ff63c9, #ff63c9);
}
.base2:before{
	content: 'Rose Pink';
	position: relative;
	color: #f1fcfe;
	color: #f1fcfe;
	font-family: 'Dancing Script', cursive;
	font-size: 15px;
	bottom: -50px;
	right: -10px;

}
.tip3{
	background-image: linear-gradient(#e11584, #e11584, #e11584);	
}
.base3:before{
	content: 'Magenta';
	position: relative;
	color: #f1fcfe;
	color: #f1fcfe;
	font-family: 'Dancing Script', cursive;
	font-size: 20px;
	bottom: -50px;
	right: -10px;
}
.tip4{
	background-image: linear-gradient(#906355, #906355, #906355);
}
.base4:before{
	content: 'Taupe';
	position: relative;
	color: #f1fcfe;
	color: #f1fcfe;
	font-family: 'Dancing Script', cursive;
	font-size: 20px;
	bottom: -50px;
	right: -20px;
}
.tip5{
	background-image: linear-gradient(#fde5b5, #fde5b5, #fde5b5)
}
.base5:before{
	content: 'Peach';
	position: relative;
	color: #f1fcfe;
	font-family: 'Dancing Script', cursive;
	font-size: 20px;
	bottom: -50px;
	right: -20px;
}
.tip6{
     background-image: linear-gradient(#f209b1, #f209b1, #f209b1);
}
.base6:before{
	content: 'Fuchsia';
	position: relative;
	color: #f1fcfe;
	font-family: 'Dancing Script', cursive;
	font-size: 20px;
	bottom: -50px;
	right: -15px;
}
@media only screen and (max-width:600px){
  /*Mobile phone responsiveness*/
  body{
    width: ;
  }
  h3{
    font-size: 28px;
    color: white;
    position: absolute ;
    left: 100px;
  }
  h2{
    font-size: 28px;
     position: absolute ;
    left: 90px;
   bottom: -35px;
      color: gold;
  }
}
@media only screen and (min-width:700px){
  /*for laptop responsiveness*/
 
}
