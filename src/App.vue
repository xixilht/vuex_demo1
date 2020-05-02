<template>
  <div>
    <!-- 以标签形式使用组件 -->
    <my-addition></my-addition>

    <p>---------------------------------</p>

    <my-subtraction></my-subtraction>
  </div>
</template>

<script>
// 导入了两个组件
import Addition from './components/Addition.vue'
import Subtraction from './components/Subtraction.vue'

export default {
  data() {
    return {}
  },
  // 希望把上面导入的组件注册为App的私有子组件
  components: {
    // 建议把组件都改造成'连字符'的形式
    'my-addition': Addition,
    'my-subtraction': Subtraction
  }
}
</script>
