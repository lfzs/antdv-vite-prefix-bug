
1、pnpm install && pnpm dev 启动项目
2、访问 http://localhost:5173/
3、collapse 展开/折叠动画消失
4、移除 App.vue 文件中 a-config-provider 的 prefixCls 属性，动画正常

```js
// App.vue
// 一旦指定 prefixCls 则 collapse 展开和折叠动画没了
// 移除 prefixCls 则正常
<a-config-provider prefixCls="kkk">
  <a-collapse>
    <a-collapse-panel key="h1" header="This is panel header 1">1</a-collapse-panel>
    <a-collapse-panel key="h2" header="This is panel header 2">2</a-collapse-panel>
    <a-collapse-panel key="h3" header="This is panel header 3">3</a-collapse-panel>
  </a-collapse>
</a-config-provider>
```