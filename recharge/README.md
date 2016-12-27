### 充值页面练习 ###

#### 1. 使用模板引擎渲染页面
参考资料： [artTemplate.js](https://github.com/aui/artTemplate)

  ```html
  <!-- 渲染数据 -->
  <script id = "test" type="text/html">
  <div class="{{recharge.id}}">
    <p>{{recharge.type}}</p>
    <ul> 
      {{each recharge.list as value i}}
      <li class="item" data-id="{{value.id}}">{{value.text}}</li>
      {{/each}}
    </ul>
  </div>
</script>
```
```js
  var data = {recharge: {
      "id": "recharge", 
      "type": "充值", 
      "list": [
        {
          "id": "100", 
          "text": "100元"
        }, 
        {
          "id": "300", 
          "text": "300元"
        }, 
        {
          "id": "500", 
          "text": "500元"
        }, 
        {
          "id": "1000", 
          "text": "1000元"
        }, 
        {
          "id": "1500", 
          "text": "1500元"
        }, 
        {
          "id": "2000", 
          "text": "2000元"
        }
      ]
    }
  };
  var html = template('test', data);
  document.getElementById('content').innerHTML += html;
  ```

### jquery selector 练习 ###


  
