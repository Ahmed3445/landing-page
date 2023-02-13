# Landing page
## overview:
I created this project after i learned the basics of HTML and CSS
## features:
clicking on the open form button,a small window will pop up to start signing in.

 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>landing page</title>

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<meta http-equiv="X-UA-Compatible" content="IE=edge" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>landing page</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
<style type="text/css">
	body {
		margin: 0;
		background-color: #cccccc;
	}
	table {
		border-spacing: 0;
	}
	td {
		padding: 0;
	}
	img {
		border: 0;
	}
    .wrapper {
		width : 100%;
		table-layout : fixed;
		background-color : #cccccc;
		padding-bottom : 60px;
	}

	.main {
		background-color : white;
		margin :  0 auto;
		width  :  100%;
		max-width : 600px;
		border-spacing : 0 ;
		font-family:sans-serif ;
		color: black;
	}
	.center {
        margin-left: auto;
        margin-right: auto;
        display: block;
        width: 50%;
		padding-left: 40px;
		
		
		
    }

	.two-columns{
		text-align: right;
		font-size: 0;
	}
	.two-columns .column {
		width: 100%;
		max-width: 300px ;
		display: inline-block;
		vertical-align: top;
		
	}
	 .two-columns .content {

		font-size:15px; 
	  line-hight: 20px;	
	  text-align:left;

	 }

	 input[type=text] {
  
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 2px solid red;
  border-radius: 4px;
  
}
input[type=email] {
  
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border: 2px solid red;
  border-radius: 4px;
  
}
.form{
    border: 10px solid red;
} 
.button{
	   background-color:blue;
	   color:white;
	   text-decoration:none;
	   padding: 12px  12px;
	   font-weight:bold;
	   border-radius:5px;	
	}
.open-button {
  background-color: #555;
  color: white;
  padding: 16px 20px;
  border: none;
  cursor: pointer;
  opacity: 0.8;
  position: fixed;
  bottom: 23px;
  right: 28px;
  width: 280px;
}

.form-popup {
	display: none;
  position: fixed;
  bottom: 0;
  right: 15px;
  border: 3px solid #f1f1f1;
  z-index: 9;
}



.form-container input[type=text], .form-container input[type=email] {


	width: 100%;
  padding: 15px;
  margin: 5px 0 22px 0;
  border: none;
  background: #f1f1f1;

}

/* When the inputs get focus, do something */
.form-container input[type=text]:focus, .form-container input[type=email]:focus {
  background-color: #ddd;
  outline: none;
}


 



</style>
</head>
<body>


<center  class="wrapper">
 <table class="main" width="100%">
<!-- LOGO SECTION -->
   <tr>
    <td>
		<table width="100%">

		<h1 style="font-family: Sofia, sans-serif ; color: gold; " class="center">
			web design
		</h1>

	    </table>

    </td>
   </tr> 


<!-- TWO COLUMN SECTION -->

<tr>
	<td style="padding: 14px 0 4px ;">
		<table width="100%">

			<tr>
				<td class="two-columns">

					<table class="column">
						<tr>
							<td style="padding: 0 62px; 10px">
								
								<img src="web-design.png" alt="image" width="200">
							</td>
						</tr>
					</table>

					<table class="content">
						<tr>
							<td  style="padding: 0 62px; 10px">
							 
								<h2>
								create custome designs
							    </h2>
								<h3>over the years we have built up a 
								massive portfolio our client website
								and email designs.</h3>
								<h3>
								we would love to share them with you,
								get to know our work</h3>

							</td>
						</tr>
					</table>
				</td>


				
				
			</tr>

		</table>
	</td>
</tr>

<!-- A button to open the popup form -->
<button class="open-button" onclick="openForm()">Open Form</button>
	 

<!-- form -->


<tr>
    <td>
		<table width="100%">

			<fieldset style="background-color:gold ;" class="form-popup" id="myForm">
				<form action="/action_page.php">
					<label for="fname">Name</label>
					<input type="text" id="fname" name="fname"><br>
					<label for="Email">Email</label>
					<input type="email" id="Email" name="Email"><br>
			</form><br>


	   
			<a href="#" class="button"> sign up</a>
				
				<button type="button" class="btn cancel" onclick="closeForm()">Close</button>

			</fieldset>
 

	    </table>

    </td>
   </tr> 



 <script>
	function openForm() {
	  document.getElementById("myForm").style.display = "block";
	}
	
	function closeForm() {
	  document.getElementById("myForm").style.display = "none";
	}
	</script>









</table> 
</center>







</body>
</html>
