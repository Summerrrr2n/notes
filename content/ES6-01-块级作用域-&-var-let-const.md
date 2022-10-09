Title: ES6-01 块级作用域 & var/let/const
Date: 2022-04-08 11:56:15
Tags: note, 学习, 学习, 工作, 深入理解ES6

<!-- wp:heading {"level":3} -->
<h3>目的： </h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>为了防止var的变量提升导致的bug，使js更加灵活</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>内容：</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>ES6 引入了块级作用域，将let、const的作用域限制在当前代码块中（函数内部/{和}之间的区域）</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>let </strong>用于代替var声明变量，同一最小作用域中不能重复声明变量</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>const</strong> 用于声明常量，同一最小作用域中不能重复声明变量，const声明时必须进行初始化赋值，一旦其值被设定后不能再更改。当const常量为对象时，可以访问修改其属性值。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>优点：</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>可以将计数器变量限制在循环内部，适用于for、for-in、for-of</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>更安全，let const可以创建新的全局绑定，不会改变全局对象的属性，例如window对象的属性，而var会</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>缺点：</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>var 声明在扫描代码时会被提升至作用域顶部</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>let const 声明在扫描代码时会被放入临时死区中，执行了声明语句之后才能从临时死区中移出，因此在变量声明前访问时会引发引用错误，即使是较为安全的typeof</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>最佳实践：</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>默认使用const，只有确实需要改变变量的值时才是用let，大部分的值在初始化之后不应再改变</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->
