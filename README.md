# simple-animation-
利用观察者模式制作多场景动画
用法 example

给每个场景对象订阅一个"完成"的事件，然后在每个场景运行结束发派发这个"完成事件"

订阅场景pageA完成事件  
observer.subscribe("completeA", function() {
                                   //做一些是
                                   })
触发场景pageA完成事件 
new pageA(function() {
    observer.publish("completeA"); //触发
})
