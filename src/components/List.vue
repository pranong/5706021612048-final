<template>
  <div class="hello">
    <table class="table">
      <tbody>
        <tr>
          <th scope="row">{{index+1}}</th>
          <td>{{list.name}}</td>
          <td>{{list.phone}}</td>
          <td>{{list.email}}</td>
          <td>  <button @click="remove(index)" class="btn btn-danger" >Delete</button></td>
        </tr>

      </tbody>
    </table>


  <!-- {{list.name}}
  {{list.phone}}
  {{list.email}}
    <button @click="remove(index)">X</button>
  </div> -->
</template>

<script>
export default {
  props: ['list', 'remove', 'index'],
  data () {
    return {

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
