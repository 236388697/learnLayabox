###流程
 > 初始化舞台 初始化列表 往列表里添加显示对象 显示对象调用运动方法 增加鼠标监听 当触发监听的时候 回调切割水果类

###西瓜类

属性：{
    img，
    x，
    y 
}
方法 运动曲线 （x，y）{
  //给对象添加一个运动曲线  

}
方法 切割水果 （x，y）{
    //换切割后的图片
    //重新计算运动曲线
}

监听此对象的鼠标事件 当鼠标划入水果对象时候 处发切割水果（）
```
	//增加鼠标事件
		rect.on(Event.MOUSE_DOWN, this, mouseHandler);
		rect.on(Event.MOUSE_UP, this, mouseHandler);
		rect.on(Event.CLICK, this, mouseHandler);
		rect.on(Event.RIGHT_MOUSE_DOWN, this, mouseHandler);
		rect.on(Event.RIGHT_MOUSE_UP, this, mouseHandler);
		rect.on(Event.RIGHT_CLICK, this, mouseHandler);
		rect.on(Event.MOUSE_MOVE, this, mouseHandler);
		rect.on(Event.MOUSE_OVER, this, mouseHandler);
		rect.on(Event.MOUSE_OUT, this, mouseHandler);
		rect.on(Event.DOUBLE_CLICK, this, mouseHandler);
		rect.on(Event.MOUSE_WHEEL, this, mouseHandler);
```


###舞台
```
舞台api
Laya.stage

	// 不支持WebGL时自动切换至Canvas
		Laya.init(Browser.clientWidth, Browser.clientHeight, WebGL);

		Laya.stage.alignV = Stage.ALIGN_MIDDLE;
		Laya.stage.alignH = Stage.ALIGN_CENTER;

		Laya.stage.scaleMode = "showall";
		Laya.stage.bgColor = "#232628";

		setup();
```
###显示对象 



###显示列表
```
//列表节点
laya.display.Sprit
```
