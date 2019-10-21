10.21日测验
在本地创建一个文件夹叫test10.21 ,文件夹中应含有5个html文件,分别命名为1.html等.再创建一个readme.txt文件,将这几个问题贴如其中,最后将html中的js代码贴到答的下方.

1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答: 
     	<div id="h1"></div>
		<script type="text/javascript">
			var a="abc"
			var b="123"
			var h1=document.getElementById("h1")
		    h1.innerHTML=a+b
			
		</script>

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:
<div id="h3"></div>
	
		<script type="text/javascript">
			var h3 =document.getElementById("h3")
			var num ="79387.348";
			var num2 =num.substr(0,8);
			console.log(num2)
			h3.innerHTML=num2
			
		</script>

4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:
<div id="h4">
			
		</div>
		<img src="img/head/icon/1.jpg"/ id="img">
		<script type="text/javascript">
			var h4 =document.getElementById("h4")
			var img =document.getElementById("img")
			var urls =img.getAttribute("src")
			console.log(urls)
			h4.innerHTML=urls
		</script>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:<div id="h5">	</div>
		<script type="text/javascript">
			var h5 =document.getElementById("h5")
			var num =prompt("请输入验证码")
			if(num.value==true){
				h5.innerHTML=num.value.toUpperCase() 
			}
			
		</script>