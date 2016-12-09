<template>
 <ul class='listBox'>
 <li class='list' v-for='item in list'>{{item.text}}</li>
 </ul>
</template>

<script>
export default {
  name: 'ListBox',
  data () {
    return {
      list: [{img: '', text: 'xxxx'}, {img: '', text: 'xxxx'}, {img: '', text: 'xxxx'}]
    }
  }
}
</script>
