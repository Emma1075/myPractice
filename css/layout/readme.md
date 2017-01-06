

## 1.圣杯布局与双飞翼布局
[千玺圣杯布局与双飞翼布局](https://theqwang.github.io/2016/01/08/%E6%B5%85%E6%9E%90%E5%9C%A3%E6%9D%AF%E5%B8%83%E5%B1%80%E5%92%8C%E5%8F%8C%E9%A3%9E%E7%BF%BC%E5%B8%83%E5%B1%80/)

## 2.flex 布局


用flex布局：

1. 最外层`display: flex`;

2. 用`order: -1`控制左右顺序

3. 内容部分自适应，设为`flex-grow: 1`

html 结构
```html
  <header>header</header>
    <div class="container">
      <div class="main">main</div>
      <div class="sub">sub</div>
      <div class="extra">extra</div>
    </div>
  <footer>footer</footer>
```

css 代码

```css
  .container {
    display: flex;
    min-height: 30vh;
  }

  .main {
    flex-grow: 1;
    background-color: #F4F4F4;
  }

  .sub {
    order: -1;
    width: 12em;
    background-color: #fcc;
  }

  .extra {
    width: 10em;
    background-color: #EED5B7;
  }

```
> 参考：[详解 flex-grow 与 flex-shrink](https://zhuanlan.zhihu.com/p/24372279);
[flex语法篇-阮一峰](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html)；
[flex教程-阮一峰](http://www.ruanyifeng.com/blog/2015/07/flex-examples.html);
