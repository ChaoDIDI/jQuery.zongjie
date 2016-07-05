# jQuery.zongjie

```txet


1.jQuery的元素选择器
    //jQuery元素选择器返回的一个jQuery对象(也简称jQuery容器)
    原生的js元素选择器返回的是一个标签
    1).$("#id")//根据id选择一个元素,如$("#app")选择id为app的标签,返回一个jQuery对象
        如果需要获取标签信息,可以使用$("#app").get(0)
    2).$(".className")//根据class选择多个元素 返回一个jQuery对象(jQuery数组对象)
        如$(".li-item")选择所有class="li-item"的元素.
            我们可以通过each方法遍历所有选中的标签$(".li-item").each(function(){ $(this)//this表示当前标签,通过$(this)把当前标签转换为jQuery对象})
            $("tagName")//根据tagName(标签名字)选择多个元素
            //联合查找,通过标签.id.classname等的结合对元素进行精确查找
            //联合查找和css样式中的联合查找用法基本类似
            $("div.classname")//查找class="className"的所有div
            $("#div.classname")//查找所有id为div的元素的内部的所有class="classname"的元素
            $(".li-item[data-val]")//查找所有包含data-val属性并且class="li-item"的元素
            $(".li-item[name='grade']")//查找所有name="grade"并且class="li-item"的元素
2.jQuery的事件绑定

 为所有ID为btn的元素添加click事件

 方式一
 $("#btn").click(function(){
 })
 方式二
 $("#btn").bind("click",function(){
 })
3.jQuery标签元素的基本操作(属性.样式)

$("#userName").attr("name")//获取标签的name属性
$("#userName").attr("name","小彪")//设置标签的name属性


//通过.text获取或者设置标签的文本内容

//通过.html获取或者设置标签的html元素内容

//通过.data获取设置标签的dataset内容

4.jQuery.validate 表单验证插件(是实际开发中使用率最高的一款)
5.jQuery.fullScreen 全屏插件
6.jQuery.jGrowl 弹出提示插件(tip)(效果:http://www.mafengwo.com)
```
