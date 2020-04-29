# 每周总结可以写在这里

小技巧  三目嵌套： {{item.errorField == 1 ? item.email== "" ? '邮箱为空' :"格式不正确" : item.email}}
对象不可哈希

Completion Record   
    [[type]}: normal,break , continue ,return ,or throw
    [[value]]: Types
    [[target]]: label 

简单语句 ：

复合语句：

iteration
    while
    do whild()
    for( ; ; ;)
    for( variable  in  object )  循环遍历一个对象所有属性
    for( of )    在（包括 Array，Map，Set，String，TypedArray，arguments 对象等等）上创建一 个迭代循环，调用自定义迭代钩子，并为每个不同属性的值执行
    var
    const /  let 
    in 
for() 本身会产生作用域
try 语句使您能够测试代码块中的错误。
catch 语句允许您处理错误。
Throw "sdfsdf" 语句允许您创建自定义错误。  或者 throw new Error("收待发放.")
finally 使您能够执行代码，在 try 和 catch 之后，无论结果如何。


<input id="demo" type="text">
<button type="button" onclick="myFunction()">测试输入</button>
<p id="message"></p>


<script>
function myFunction() {
    var message, x;
    message = document.getElementById("message");
    message.innerHTML = "";
    x = document.getElementById("demo").value;
    try { 
        if(x == "") throw "空的";
         if(isNaN(x)) throw "不是数字";
         x = Number(x);
        if(x < 5) throw  "太小";
        if(x > 10) throw "太大";
    }
    catch(err) {
        message.innerHTML = "输入是 " + err;
    }
}

Interatil 
function* foo(){
} 