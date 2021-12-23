<template>
  <div id="app" class="page_wrap">
	<div class="page_header">
		<div class="content">
			<div class="text bold">Марина Звёздная</div>
		</div>
		<HelloWorld msg="Welcome to Your Vue.js App"/>
	</div>
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
