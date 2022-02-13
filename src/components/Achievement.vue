<template>
<div>
  <modal 
  name="example"
  shiftX= '0.98'
  shiftY = '0.02'
  width = "20%"
  height = "10%"
  >
  This is an example
  </modal>
</div>
</template>

<script>
export default {
    name: 'MyComponent',
    mounted () {
        this.$modal.show('example')
    }
}
</script>


