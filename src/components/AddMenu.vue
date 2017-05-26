<template>
  <div class="hello">
    <div class="col-lg-6">
     <div >
       <input v-model="name" type="text" class="form-control" placeholder="Name" width="200"></input>
       <input v-model="phone" type="text" class="form-control" placeholder="Credits" width="200"></input>
       <input v-model="email" type="text" class="form-control" placeholder="Grade" width="200"></input>

     </div><!-- /input-group -->
              <button @click="add(name, phone, email)" class="btn btn-default btn-lg" type="button">
                <span class="glyphicon glyphicon-plus" aria-hidden="true"></span>
              </button>
   </div><!-- /.col-lg-6 -->
  </div>
</template>

<script>
export default {
  props: ['add'],
  data () {
    return {
      input: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>
