# Html5
html5&amp;CSS&amp;JS
<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8" />
	<title>根据不同的窗口尺寸来选择使用不同的样式的示例</title>
	<style type="text/css">
		body{
			margin: 20px 0;
		}
		#container{
			width: 960px;
			margin: auto;
		}
		#wrapper{
			width: 740px;
			float: left;
		}
		p{
			height: 600px;
			line-height: 50px;
			text-align: left;
			margin: 0 0 20px 0;
		}
		span{
			line-height: 20px;
		}
		.a{
			font-weight: bold;
		}
		#img{
			margin-left: auto;
			margin-right: auto;
		}
		#main{
			width: 520px;
			float: right;
			background: yellow; /* 黄色 */
		}
		#sub01{
			width: 200px;
			float: left;
			background: #FFEEAA;
		}
		#sub02	{
			width: 200px;
			float: right;
			background: #009ACD;
		}
		
		/* 窗口宽度在800px以上 */
		@media screen and (min-width: 800px) {
			/* 3栏显示*/
			#container{
				width: 1000px;
			}
			#wrapper{
				width: 780px;
				float: left;
			}
			#main{
				width: 560px;
				float: right;
			}
			#sub01{
				width: 200px;
				float: left;
			}
			#sub02{
				width: 200px;
				float: right;
			}
			span{
			line-height: 20px;
		}
		}
		
		/* 窗口宽度在800px以下 */
		@media screen and (max-width: 800px) {
			/* １栏显示  */
			#container{
				width: 100%;
			}
			#wrapper{
				width: 100%;
				float: none;
			}
			body{
				margin: 20px;
			}
			p{
				line-height: 50px;
			}
			#main{
				width: 100%;
				float: none;
			}
			#sub01{
				width: 100%;
				float: none;
				line-height: 100px;
			}
			#sub02{
				width: 100%;
				float: none;
				line-height: 100px;
			}
		}
	</style>
</head>
<body>
	<div id="container">
		<div id="wrapper">
			<p id="sub01">
				<span>
					HTML5<br />
					css3<br />
					bootstrap<br />
					others
				</span>
			</p>
			<p id="main">
				<span>
				<span >
					<br  />
						<font size="15px"><b>HTML5</b></font><br />
					万维网的核心语言、标准通用标记语言下的一个应用超文本标记语言（HTML）的第五次重大修改<br />
					<span id="img"><img src="1494728438(1).png" width="560px" /></span>
				</span>
		</div>
		<p id="sub02">
			<span class="a">What?</span><br />
			Hyper Text Markup Language<br />
			<span class="a">Where?</span><br />
			In the vebsite<br />
			<span class="a">Price?</span><br />
			The technology is free!			
		</p>
	</div>
</body>
</html>
