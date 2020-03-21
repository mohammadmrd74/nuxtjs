<template>
  <div>
    <h1>
      this a post {{id}}
    </h1>
  </div>
</template>

<script>
export default {

  name : 'as',
  data:function() {
    return {
      id: this.$route.params.id,
      posts: [
        {
        id: '1',
        content: 'ali'
      },
      {
        id: '2',
        content: 'ali2'
      },
      {
        id: '3',
        content: 'ali3'
      },
      ]
    }
  },
  created (){
    console.log(this.id);
    
  }
}
</script>
