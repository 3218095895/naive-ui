# 使用 Dialog 预设的插槽

插槽也会随着预设变动。

```html
<n-button @click="showModal = true"> 来吧 </n-button>
<n-modal v-model:show="showModal" preset="confirm" title="Dialog">
  <template #header>
    <div>标题</div>
  </template>
  <div>内容</div>
  <template #action>
    <div>操作</div>
  </template>
</n-modal>
```

```js
export default {
  data () {
    return {
      showModal: false
    }
  }
}
```
