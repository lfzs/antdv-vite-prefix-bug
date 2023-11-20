<template>
<div style="display: flex;">
  <div>
    <h2>修改 prefixCls 展开/折叠 动画无效</h2>
    <a-config-provider prefixCls="kkk">
      <a-menu style="width: 600px" mode="inline" :items="items" />
    </a-config-provider>
  </div>

  <div>
    <h2>未修改 prefixCls 展开/折叠 动画正常</h2>
    <a-config-provider>
      <a-menu style="width: 600px" mode="inline" :items="items" />
    </a-config-provider>
  </div>
</div>

</template>
<script setup>
const items = [
  {
    key: 'one',
    label: 'Navigation One',
    title: 'Navigation One',
    children: [
      {
        key: 'option1',
        label: 'Option 1',
        title: 'Option 1',
      },
      {
        key: 'option2',
        label: 'Option 2',
        title: 'Option 2',
      }
    ],
  },
]
</script>