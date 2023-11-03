<template>
  <img alt="Vue logo" src="./assets/logo.png" />

<label for="namr"> Enter Name</label>
<input type="text" ref="newName"/>
<input type="submit" @click="test" />

  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <MyHelloWord :name="name" :family="family" :age="age" @nameClicked="test" /> -->
  <!-- <MyHelloWord
    @click="test"
    :name="name"
    :family="family"
    :age="age"
    ref="MyHelloWordComponent"
  >
    <template v-slot:Mohsen>
      <h1>Mohsen</h1>
    </template> 
<template v-slot:parsa>
  <h1>parsa</h1>
</template>
<template v-slot:age>
  <h1>30</h1>
</template>
 
    <slot>lk</slot>
</MyHelloWord> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import MyHelloWord from "./components/MyHelloWord.vue";

export default {
  data() {
    return {
      name: "Mohsen",
      family: "Jafari",
      age: 20,
    };
  },
  methods: {
    test() {
      // console.log("test" +" "+text);
      // this.$refs.MyHelloWordComponent.alertname();
     this.name= this.$refs.newName.value;
    },
  },
  watch :{
name(newValue,oldValue)
{
console.log(oldValue);
console.log(newValue);
},
  },

  name: "App",
  components: {
    // HelloWorld
    // MyHelloWord,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
