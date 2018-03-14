###流程
 > 舞台
​ 舞台是显示游戏元素的平台，在游戏视觉编程里，一切游戏的元素必须添加到舞台才能被显示。因此，舞台也是放置显示对象的最终容器。
​ 同时，舞台也是一种可以显示的对象，从编程的角度讲，任何对象都具有属性和行为。如，舞台对象具有宽、高、帧频等属性，具有添加显示对象的行为。
显示对象
​ 那什么是显示对象呢？一种入门级的理解，可以认为一切在舞台上可见的东西都能被称为显示对象。但实际上，显示对象既包括了可见的图形、文字、图片、视频等，也包括不可见的音频和显示对象容器等。
显示列表
​ 显示对象在舞台上显示之前，还需要有一个过程，那就是先添加到显示列表中。显示列表的作用就是将显示对象进行数据索引，用于层级的显示顺序（后添加的在最上层显示），然后在舞台上显示。
 
 
``` 
 初始化舞台=> 初始化列表 =>往列表里添加显示对象=> 增加鼠标监听 =>显示对象调用运动方法=> 当触发监听的时候 =>回调切割水果类
```
###显示对象 --西瓜类


属性：{
    img，
    x，
    y 
}


方法 运动曲线 （x，y）{
  //给对象添加一个运动曲线  

}
https://ldc.layabox.com/doc/?nav=zh-as-1-3-0 //显示与切换图片 api
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



###显示列表
```
//列表节点
laya.display.Sprit

https://layaair.ldc.layabox.com/api/?category=Core&class=laya.display.Sprite
```
