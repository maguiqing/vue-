<template>
  <div class="hello">
     <div @click="handleClick" class="dell">{{name}}</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      name: 'hello world'
    }
  },
  methods:{
    handleClick:function(){
        this.name='byebye world'
    }
  }
}
</script>

<style scoped>
     .dell{
      color:red;
     }
</style>
