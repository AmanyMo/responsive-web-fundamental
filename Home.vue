<template>
  <div class="home container">
    <HelloWorld />
    <div class="row">
      <div class="col-xl-3 col-md-6">
        <div class="card bg-primary text-white mb-4">
          <div class="card-body">Number of Users</div>
          <div class="card-footer d-flex align-items-center justify-content-between">
            <h4 class="small text-white stretched-link" href="#">{{numofUSERS}}View Details</h4>
          </div>
        </div>
      </div>
      <div class="col-xl-3 col-md-6">
        <div class="card bg-warning text-white mb-4">
          <div class="card-body">tracked users</div>
          <div class="card-footer d-flex align-items-center justify-content-between">
            <h4 class="small text-white stretched-link" href="#">{{numofUSER_Scrape}}View Details</h4>
            
          </div>
        </div>
      </div>
      <div class="col-xl-3 col-md-6">
        <div class="card bg-success text-white mb-4">
          <div class="card-body">Succeeded</div>
          <div class="card-footer d-flex align-items-center justify-content-between">
            <h4 class="small text-white stretched-link" href="#">{{p}}View Details</h4>
           
          </div>
        </div>
      </div>
      <div class="col-xl-3 col-md-6">
        <div class="card bg-danger text-white mb-4">
          <div class="card-body">Danger Card</div>
          <div class="card-footer d-flex align-items-center justify-content-between">
            <h4 class="small text-white stretched-link" href="#">View Details</h4>
           
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>
