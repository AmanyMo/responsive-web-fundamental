<template >
  <div>
    <h4>
      hello! here list of all msgs that we have recived
    </h4>
    <!-- use v-for -->
     <ul class="list-group  d-inline-flex p-2">
        <li class="list-group-item">
          name:amany
          <button v-on:click="open()" class="btn btn-primary">open chat</button>
        </li>
        <li class="list-group-item">
          name:asmaa
          <button  v-on:click="open()"  class="btn btn-primary">open chat</button>
        </li>
        <li class="list-group-item">
          name:Ahmed
          <button v-on:click="open()" class="btn btn-primary">open chat</button>
        </li>
      </ul>
      

     
    
  </div>
</template>

<script>
export default {
  name: "AdminDashboard",
  methods:{
    open:function(){
      this.$alert("Are you dsfsdf sure?").then(() => {
  //do something...
});
    }
  }
};
</script>

<style  scoped>
</style>