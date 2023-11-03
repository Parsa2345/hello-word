<template>
    <!-- <h1 >{{name}} {{family}} {{age}}</h1> -->

<slot name="Mohsen"></slot>
<slot name="parsa"></slot>
<slot name="age"></slot>
</template>



<script>

export default ({

    props :{
        name:String,
        family:String,
        age:Number
    },
    methods: {
        alertname(){
            alert(this.name);
            // this.$emit("nameClicked",this.name);
        }
    },
 })
</script>

<style scoped>
  h1{
    color: blue;
  }
</style>