<template>
  <div id="app">
    <!-- <HelloWorld title="slot">
      HelloWorldコンポーネントの<slot />の部分にこのテキストが入る
      <p>this is default text</p>
    </HelloWorld> -->

    <!-- 名前付きスロット -->
    <HelloWorld>
      <p>Begin</p>
      <template v-slot:first>
        First message
      </template>
      <p>Middle</p>
      <template v-slot:second>
        Second message
      </template>
      <p>End</p>
      <template v-slot:third>
        Third message
      </template>
    </HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>
