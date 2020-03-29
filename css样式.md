##微信小程序样式

####hover-class点击效果

微信小程序中，可以用 hover-class 属性来指定元素的点击态效果。

**目前支持 hover-class 属性的组件有三个：view、button、navigator。**

不支持 hover-class 属性的组件，同时也不支持 hover-stop-propagation、hover-start-time、hover-stay-time 这三个属性。

* hover-class                            类型String         none       指定按下去的样式类。当hover-class=“none”时，没有点击效果

* hover-stop-propagation     类型boolean     false        指定是否阻止本节点的祖先节点出现点击态

* hover-start-time                   类型Number     50          按住后多久出现点击态，单位毫秒

* hover-stay-time                    类型Number     400         手指松开后点击态保留时间，单位毫秒