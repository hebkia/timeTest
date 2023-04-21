<template>
  <view class="index">
    <button @tap="test">
      Hello World
    </button>
    <view>
      {{index}}
    </view>
      
      
  </view>
</template>

<script>
import { ref } from 'vue'
import './index.scss'

let i = 0

export default {

  data(){
    return {
      index:0
    }
  },
  methods:{
    test(){
      setTimeout(()=>{
        this.index = this.index + 1
      },100)
    }
  },
  setup () {
  }
}
</script>
