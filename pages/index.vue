
<script>
export default {
  data() {
    return {
     text: "",
     words: "this.text",
    }
  },
  methods: {
    onPress() {
      this.stuff = this.text;
    }
  }
}
</script>


<template>
<div>
 <h1 class="color space">Code Test</h1>
 
  <v-text-field
        v-on:value="text"
         label="Outlined"
         placeholder="Placeholder"
         outlined
       ></v-text-field>
 
  <v-btn
   v-on:click="onPress"
   elevation="2"
 >Click Here</v-btn>
 
 <p>{{ stuff }}</p>
 </div>
</template>

<style scoped>
.color {
 color: lightblue;
}

.space {
 padding-bottom: 20px;
}
</style>