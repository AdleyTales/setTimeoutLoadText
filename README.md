# setTimeoutLoadText 延时加载文字

## 代码如下

```js
	<!DOCTYPE html>
	<html>
	<head>
	<meta charset="utf-8"/>
	<title></title>
	<script src="jquery.js"></script>
	<script>
		$(function(){
			run();
		})
		
		var str="习近平新时代中国特色社会主义经济思想，是5年来推动我国经济发展实践的理论结晶，是中国特色社会主义政治经济学的最新成果，是党和国家十分宝贵的精神财富，必须长期坚持、不断丰富发展。”刚刚闭幕的中央经济工作会议，明确了以新发展理念为主要内容的习近平新时代中国特色社会主义经济思想，学懂弄通并贯彻好这一思想，是新时代推动我国经济高质量发展的基础和前提。";
		function run(){
			for(let i=1;i<=str.length;i++){
				setTimeout(function(){
					$("#sId").text(str.substring(0,i));
				},i*200);
			}	
		}
		
		function runstr(str,len){
			
		}
		
		
	</script>
	</head>
	<body>
	  <div id="sId" style="font-size:25px;"></div>
	</body>
	</html>

```