	<!DOCTYPE html>
	<html lang="en">
	<head>
	    <meta charset="UTF-8">
	    <title>电灯开关</title>
	
	</head>
	<body>
	
	<img id="light" src="20200428135921164.gif">
	
	<script>
	    /*
	        分析：
	            1.获取图片对象
	            2.绑定单击事件
	            3.每次点击切换图片
	                * 规则：
	                    * 如果灯是开的 on,切换图片为 off
	                    * 如果灯是关的 off,切换图片为 on
	                * 使用标记flag来完成
	
	     */
	
	    //1.获取图片对象
	    var light = document.getElementById("light");
	
	    var flag = false;//代表灯是灭的。 off图片
	
	    //2.绑定单击事件
	    light.onclick = function(){
	        if(flag){//判断如果灯是开的，则灭掉
	            light.src = "20200428135921164.gif";
	            flag = false;
	
	        }else{
	            //如果灯是灭的，则打开
	            light.src = "20200428135948491.gif";
	            flag = true;
	        }
	            }    
	</script>
	</body>
	</html>
	<script>
		var i=0
			if(r=current1[0]){
				i=0}
			else if(r=current[1]){
				i=1;
			}
			else if(r=current1[2]){
				i=2
			}
			else if(r=current1[3]){
				i=3
			}
			switch(i){
				case 0:
					if(r=current1[0]){
						break;
					}
					break
					case1:
					if(r=current1[1]){
						break;
					}
					break;
					case2:
					if(r=current1[2]){
						break;
					}
					break;
					default:
					if(r=current1[3]){
						break;
					}
					break;
			}
	</script>
	<script>
		var zzms=false;
    document.getElementById("td["+current1[0]+"]").addEventListener("click",function(){
  // setTimeout('document.getElementById("td["+current1[0]+"]").innerHTML="hello world"',1000);
   if(zzms){
      setTimeout('document.getElementById("td["+current1[0]+"]").innerHTML="hello world"',1000)
       zzms=false;
    }
    else{
       setTimeout('document.getElementById("td["+current1[0]+"]").innerHTML=true',1000);
        zzms=true;
    }
})
	</script>
<script>
	function testBtn(r,d,w,h,c){
		document.write("<table border='1'>")
			for(var i=0;i<r;i++){				
		document.write('<tr id="i'+i+'">')
			for(var j=0;j<d;++j){
				var s="";
				var temp=new Array()
				a=new Array(0,1,2,3,4,5)
		s=s+'<td id="j'+j+'">abc</td>';
		document.write(s)
		temp[j]=document.getElementById("j"+j)	
		temp[j].style.width=w;
		temp[j].style.height=h;
		temp[j].style.borderColor=c;
			}
			temp[i]=document.getElementById("i"+i)	
		temp[i].style.width=w;
		temp[i].style.height=h;
		temp[i].style.borderColor=c;
	document.write("</tr>")
			}
			document.write("</table>")
		}
		/*function testBtn1(){
			for(var k=0;k<6;k++){
		document.getElementsByTagName("td")[k].style.height='100px';
		document.getElementsByTagName("td")[k].style.width='100px';
		document.getElementsByTagName("td")[k].style.borderColor='red';
			}
		}*/
		testBtn(4,6,"100px","100px","red");
</script>
<body>
	<table>
		<tr>
			<td width="100px" height="100px" style="border:solid 2px greenyellow;"></td>
		</tr>
	</table>
</body>
<html>
<script>
	function example(e){
if(e.ctrlkey&&e.altkey&&e.shiftkey){
	alert('abc');
	//window.location.href='index_ok.html';
	return false
}
}
document.onkeydown=example;									
</script>
</html>
<script>
	function gosite(e){
		if(e.ctrlKey&&e.altKey&&e.shiftKey){
			alert("刚刚弹出的是鼠标右键")
			//window.location.href='each.html'
			window.open("http://www.mingrisoft.com")
			return false
			//location.reload()
		}
	}
	document.onkeydown=gosite;
</script>

