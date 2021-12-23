<template>
  <div class="page_body chat_page">
      <div class="history" v-for="messagefrom in historychat" :key="messagefrom">
          <div class="message default clearfix">
              <div class="pull_left userpic_wrap">
                  <div class="userpic userpic5" style="width: 42px; height: 42px">
                      <div class="initials" style="line-height: 42px">{{messagefrom.icon}}</div>
                  </div>
              </div>
              <div class="body">
                  <div class="pull_right date details" :title="messagefrom.date">
                      {{messagefrom.date}}
                  </div>
                  <div class="from_name">
                      {{messagefrom.from}}
                  </div>
                  <div class="text">
                      {{messagefrom.text}}
                  </div>
              </div>
          </div>
      </div>
  </div>
</template>

<script>
	import json from '@/assets/download/result.json'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
    data() {
      return {
        historychat: json,
        }
	}
}
</script>
