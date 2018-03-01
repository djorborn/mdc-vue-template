<template>
     <div>
          <Drawer/>
          <Toolbar/>
          <hr/>
          <br>
        <div class="mdc-text-field" data-mdc-auto-init="MDCTextField">
  <input class="mdc-text-field__input" type="text" id="input">
  <label for="input" class="mdc-text-field__label">Input Label</label>
  <div class="mdc-line-ripple"></div>
</div>
          <button class="mdc-button mdc-button--raised mybtn" data-mdc-auto-init="MDCRipple" mdc-ripple-is-unbounded>Button</button>
     </div>
</template>

<script>
    import Toolbar from './components/Toolbar.vue';
    import Drawer from './components/Drawer.vue';

    export default {
        name: 'app',
        data () {
            return {
                hi: 'Hello'
            }
        },
        components: {
            Toolbar,
            Drawer,
        }
    }
</script>

<style lang="scss">
   .mybtn {
       font-size: 30px;
       position: absolute;
       z-index: 4;
   }
</style>