Title: bug 调试方法
Date: 2022-04-22 11:08:05
Tags: 未分类
Category: 未分类

<!-- wp:paragraph -->
<p><a href="https://pro.ant.design/zh-CN/docs/debug">https://pro.ant.design/zh-CN/docs/debug</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>在我们的开发中，由于对底层的不理解或者兼容性的问题，很有可能会出现白屏或者 Out Of Memory 的问题，也有一些问题没有任何可以 debug 着手的方式。这时候就要用到一些 debug 的方案。</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 id="二分法定位"><a href="https://pro.ant.design/zh-CN/docs/debug#%E4%BA%8C%E5%88%86%E6%B3%95%E5%AE%9A%E4%BD%8D"></a>二分法定位</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>二分法是 debug 中最常用也是最好用的方式，非常适用于我的代码昨天还是好的和各类 Out Of Memory 报错。我们可以程序逻辑一点点注释掉，不断地进行排错，完全能把问题可能出现的范围缩小，然后找出罪魁祸首。再用常规手段调试。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>node 中 Out Of Memory 最常用的方式就是删除一半依赖，然后进行重试来不断缩小范围，直到找个问题所在。二分调试大法每次遇到棘手的 bug，基本上都能解决，程序员必备技能，无关语言。</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 id="小黄鸭法"><a href="https://pro.ant.design/zh-CN/docs/debug#%E5%B0%8F%E9%BB%84%E9%B8%AD%E6%B3%95"></a>小黄鸭法</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>处理 bug 的过程，最难的不是怎么解决问题，而是如何定位代码的 bug，如果实在是一筹莫展，尤其是算法类的问题。我们可以通过小黄鸭法来进行 debug。我们可以找任何物体也可以是同事讲一遍或者讨论一遍，当然上网发帖也是好方式。</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 id="重写一遍"><a href="https://pro.ant.design/zh-CN/docs/debug#%E9%87%8D%E5%86%99%E4%B8%80%E9%81%8D"></a>重写一遍</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>这个方法成本最高，适用于可以乱七八糟的代码，尤其是陈年代码，如果实在搞不懂修不了 bug，可以加好测试用例重新写一遍。毕竟很多的 bug 其实都是错别字。</p>
<!-- /wp:paragraph -->
