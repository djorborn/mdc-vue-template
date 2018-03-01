<template lang="pug">
  .mdc-drawer.mdc-drawer--permanent.mdc-typography
    .mdc-drawer__toolbar-spacer
    .mdc-drawer__content
        #icon-with-item-demo.mdc-list
            a.mdc-list-item.mdc-ripple-surface(
                v-for="link in links" 
                v-bind:href="link.link" 
                v-bind:class="link.active"
                data-mdc-auto-init="MDCRipple")
                i.material-icons.mdc-list-item__graphic(aria-hidden="true") {{link.icon}}
                span {{link.text}}

</template>

<script>
export default {
  name: 'Drawer',
  data () {
      return {
          links: [
              {id: 0, text: 'Home', link: '/#home', icon: 'home', active: 'mdc-list-item--activated'},
              {id: 1, text: 'About', link: '/#about', icon: 'span', active: ''},
          ],
      }
  },
  methods: {
    
  }
}
</script>

<style lang="sass">

</style>
