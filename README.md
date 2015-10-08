
#Q：判断字符串以字母开头，后面可以是数字，下划线，字母，长度为6-30
#Q：请举例使用callee属性实现函数的递归使用
------------------------------------------------------------------------------
#Q：Ajax同步和异步的区别，如何解决跨域问题?
------------------------------------------------------------------------------
#Q：apply和call方法有形似之处，请说出二者的区别
------------------------------------------------------------------------------
#Q：请解读一下javascript代码，并指出问题所在
var Obj=function(msg){
    this.msg=msg;
    this.shout=function(){
		alert(this.msg);
	}
	this.waitAndShout=function(){
    	setTimeout(this.shout, 2000);
    }
}
var aa=new Obj("abc");
aa.waitAndShout();
#Q：请给Array本地对象增加一个原型方法，他的用途是删除数组中重复的条目，并将新的数组返回
#Q：JavaScript是一门什么样的语言，它有哪些特点？
#Q：希望获取到页面中所有的checkbox怎么做？(不使用第三方框架)
#Q：当一个DOM节点被点击时候，我们希望能够执行一个函数，应该怎么做？
#Q：看下列代码输出为何？解释原因。
1
2
3	var a;
alert(typeof a);
alert(b);
#Q：看下列代码,输出什么？解释原因。
1
2	var a = null;
alert(typeof a); 
#Q：看下列代码,输出什么？解释原因。
1
2
3	var foo = "11"+2-"1";
console.log(foo);
console.log(typeof foo);
#Q：将字符串”<tr><td>{$id}</td><td>{$name}</td></tr>”中的{$id}替换成10，{$name}替换成Tony （使用正则表达式）
#Q：为了保证页面输出安全，我们经常需要对一些特殊的字符进行转义，请写一个函数escapeHtml，将 <  , > , & , “  进行转义
#Q：看下列代码，将会输出什么?(变量声明提升)
1
2
3
4
5
6	var foo = 1;
(function(){
    console.log(foo);
    
    console.log(foo);
})();
#Q：有这样一个URL：http://item.taobao.com/item.htm?a=1&b=2&c=&d=xxx&e 请写一段JS程序提取URL中的各个GET参数(参数名和参数个数不确定)，将其按key-value形式返回到一个json结构中，如{a:'1', b:'2', c:'', d:'xxx', e:undefined}。
#Q：看下面代码，给出输出结果。
	for(var i=1;i<=3;i++){
  setTimeout(function(){
      console.log(i);    
  },0);  
};
#Q：写一个function，清除字符串前后的空格。（兼容所有浏览器）
#Q：下面这个ul，如何点击每一列的时候alert其index?（闭包）
1
2
3
4
5	<ul id=”test”>
<li>这是第一条</li>
<li>这是第二条</li>
<li>这是第三条</li>
</ul>
#Q：给String对象定义一个repeatify方法。该方法接收一个整数参数，作为字符串重复的次数，最后返回重复指定次数的字符串。例如：
1	console.log('hello'.repeatify(3));
输出应该是
1	hellohellohello.
Q：以下哪条语句会产生运行错误： 
A.var obj = ();           B.var obj = [];        C.var obj = {};        D.var obj = //; 
第一个；
2.定义数组；
3.定义对象；js中对象：方法和属性的一个集合，
{
property1:statement,
property2:statement2,
propertyN:statmentN
}
4.定义正则；

Q：给Array原型添加一个方法,这个方法接受一个参数,如果这个参数在数组中存在那么就把它从数组中删除。
Q：对下面这个对象进行克隆. var student = { name:”zhang3″, sno:”20080328″, age:”20″, call:function(){alert(this.name+this.sno+this.age);} };
Q：请问p.name是多少？
var fun = function(){
this.name = 'peter';

return {
name: 'jack'
};
}
var p = new fun();
Q：请问a.info.name和b.info.name分别是多少？
var fun = function(){

}
fun.prototype = {
info : {
name : 'peter',
age : 25
}
}
var a = new fun();
var b = new fun();
a.info = {};
a.info.name = 'jack';
b.info.name = 'tom';

Q：写一个traverse函数，输出页面所有宽度和高度大于50像素的节点。
Q：填写内容让a.name 等于“name1” 让 b.name 等于“name2”
function obj(name){
    1 
}
obj.  2 = "name2";
var a = obj("name1");
var b = new obj;
1: 

Q： javascript 语言特性中，有很多方面和我们接触的其他编程语言不太一样，比如说，javascript语言实现继承机制的核心就是  1  (原型)，而不是Java语言那样的类式继承。Javascript 解析引擎在读取一个Object的属性的值时，会沿着  2  (原型链)向上寻找，如果最终没有找到，则该属性值为  3  undefined； 如果最终找到该属性的值，则返回结果。与这个过程不同的是，当javascript解析引擎执行“给一个Object的某个属性赋值”的时候，如果当前Object存在该属性，则改写该属性的值，如果当前的Object本身并不存在该属性，则赋值该属性的值 。


