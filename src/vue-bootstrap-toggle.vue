<template>
  <div class="toggle btn {{ size + ' ' + style }}" data-toggle="toggle"
       :class="{ 'btn-'+ onstyle: checked, 'btn-' + offstyle + ' off': !checked }">
    <input type="checkbox" data-toggle="toggle" v-model='checked'>
    <div class="toggle-group">
      <label class="btn {{ 'btn-'+ onstyle + ' ' + size + 'toggle-on' }}">
        {{ on }}
      </label>
      <label class="btn {{ 'btn-'+ offstyle + ' ' + size + ' active toggle-off' }}">
        {{ off }}
      </label>
      <span class="toggle-handle btn btn-default {{ size }}"></span>
    </div>
  </div>
</template>

<script>
const sizes = new Map([
    ['mini', btn-xs'],
    ['small', btn-sm'],
    ['large', btn-lg'],
])

/* TODO: styles on toggle div, and labels */
export default {
    data() {
        return {
            on: 'On',
            off: 'Off',
            onstyle: 'primary',
            offstyle: 'default',
            size: 'normal',
            style: '',
            width: null,
            height: null,
            checked: false,
        }
    }

    computed: {
        size() {
            return sizes.get(this.size) || ''
        },
    }

    methods {
        toggle(){}
        on){}
        off(){}
        enable(){}
        disable(){}
        trigger(){}
    }
}
</script>

<style>
</style>
