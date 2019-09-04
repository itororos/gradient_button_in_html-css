# gradient_button_in_html-css
<!DOCTYPE html>
<html>
<head>
	<title>buttons_catalogue</title>
	<style type="text/css">
		/* this is a body*/
		body{
			background-color: black;
		}
		.container1{/*a container is required to partition the screenspace*/
			text-align: center;
			margin-top: 100px;
		}
		.btnB{
			position: absolute;
			top: 25%;
			left: 50%;
			transform: translate(-50%,-50%);
			font-size: 30px;
			padding: 10px 60px;
			border-radius: 45px;
			background: linear-gradient(90deg,#fb0094,#0000ff,#00ff00,#ff0000);/*linearly changes color according to the specified hex*/
			animation: animate 80s linear infinite;
			font-family:"sans-serif";
			color: white;
			background-size: 400%;
		}
        @keyframes animate{
        	0%{
        		background-position: 0 0;
        	}
        	25%{
        		background-position: 400% 0;
        	}
        	50%{
        		background-position: 400% 0;
        	}
        	100%{
        		background-position: 0 0;
        	}

        }
	</style>
</head>
<body>
  <div class ="container1">
  	
  	<button class="btnB"> btnB</button>
  	
  </div>
</body>
</html>
