# img_loading
<h1>图片预加载</h1>

<dl>图片预加载分为两种方式：
  <dd><strong>1、预先加载：</strong>
        <div>原理：先加载第一张图片，在客户观看第一张图片时加载其余图片</p><p>需要用到 new Image(),设置图片对象的src</p></div></dd>
  <dd><strong>2、按需加载：</strong>
        <div>原理：加载出现在可视区的图片，创建一个方法,当图片距离顶部的距离 < 页面滚动距离 + 可视区高度时页面 ,将图片的自定义属性data-src的值设置给src</p>
        <p>需要用到自定义属性 data-name，以及获取自定义属性 obj.dataset.name,
        这里涉及到一个优化方案，可在代码中查看</p></div></dd>
</dl>
