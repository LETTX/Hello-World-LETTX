# Hello-World-LETTX
Crossing the hills, someone is waiting

//添加div
function createDiv(iWidth, iHeight) {
	var oDiv = document.createElement("DIV");
	with (oDiv.style) {
		width = iWidth + "px";
		height = iHeight + "px";
		position = "absolute";
		left = "50%";
		top = "50%";
		marginLeft = -(iWidth / 2) + "px";
		marginTop = -(iHeight / 2) + "px";
		paddingTop = 15 + "px";
		textAlign = "center";
		zIndex = 9999;
		borderRadius="10px";
		//测试给他加个背景
		backgroundColor = "white";

	}
	return oDiv;
}

//////////////////////////////////////
var oDiv = createDiv(120, 40);
document.body.appendChild(oDiv);
oDiv.innerHTML = '下发指令成功';

setTimeout(function(){
 document.body.removeChild(oDiv);
},1000)
