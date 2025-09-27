<script>
export default { 
  data() {
    return {
      id: "demo1",
      blueBoth: true 
    }
  },
  methods: { 
    changecolor() {
      this.blueBoth = !this.blueBoth;
    }
  }
}
</script>

<template>
  <div class="container">
    <div 
      v-bind:id="id" 
      class="m-2" 
      v-bind:class="{ blueBox: blueBoth, redBox: !blueBoth }"
    >
      div ID : {{ id }}
    </div>

    <button 
      type="button" 
      v-bind:class="{ 'btn btn-secondary': blueBoth, 'btn btn-danger': !blueBoth }"
      @click="changecolor"
    >
      Change Color
    </button>
  </div>
</template>

<style scoped>
.redBox {
  background-color: red;
}
.blueBox {
  background-color: blue;
}
#demo1 {
  color: white;
}
</style>
