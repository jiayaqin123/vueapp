<template>
    <div>
        <div class='menu'>
            <input v-model='keyWords' v-on:blur="blurs" v-on:focus='focus'>
        </div>
        <ul class="history">
            <li v-for='list in history'>{{list}}</li>
        </ul>
        <ul class="guides">
            <li v-for='i in guides'>{{i.text}}</li>
        </ul>
    </div>

</template>

<script>
export default {
  name: 'InputBar',
  data () {
    return {
      keyWords: 'keywords',
      history: [ 1, 2, 3, 4 ],
      guides: [{val: '1', text: '创意菜'}, {val: '1', text: '创意菜'}, {val: '1', text: '创意菜'}]
    }
  },
  methods: {
    blurs () {
      document.getElementsByClassName('history')[0].style.display = 'none'
    },
    focus () {
      document.getElementsByClassName('history')[0].style.display = 'block'
    }
  }
}
</script>
