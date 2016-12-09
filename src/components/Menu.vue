<template>
 <ul class='menu'>
   <li v-for='menu in menus'><i>{{ menu.icon }}</i><span>{{ menu.text }}</span></li>
 </ul>
</template>

<script>
export default {
  name: 'AppMenu',
  data () {
    return {
      menus: [{icon: 'icon', text: 'menu'}, {icon: 'icon', text: 'menu'}, {icon: 'icon', text: 'menu'}]
    }
  }
}
</script>
