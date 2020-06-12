<template>
  <div class="message container">
    <h1>This is about Messages & Suggestions</h1>
    <ul>
      <!-- edit using v-for to make #of cards =#of msgs-->

      <li>
        <div class="overflow-auto card m-3 border-info" style="width: 18rem;">
          <div class="card-body">
            <h5 class="card-title">amany</h5>
            <h6 class="card-subtitle mb-2 text-muted">1661</h6>
            <p class="card-text">
              {{msg}}GOOD Some quick example text to build the bulk of the card's content example
              text to build the bulk of the card's
              contentexample text to build the bulk of the card's
              contentexample text to build the bulk of the card's contentexample text
              to build the bulk of the card's content.
            </p>
            <button v-on:click="reply()" class="card-link btn btn-dark">Reply</button>
            <button v-on:click="ok()" class="card-link btn btn-dark">Ok</button>
          </div>
        </div>
      </li>

      <v-divider></v-divider>
      <li>
        <div class="card m-3 border-info" style="width: 18rem;">
          <div class="card-body">
            <h5 class="card-title">AMANY ..</h5>
            <h6 class="card-subtitle mb-2 text-muted">5000</h6>
            <p
              class="card-text"
            >{{msg}}GOOD Some quick example text to build the bulk of the card's content.</p>
            <button v-on:click="reply()" class="card-link btn btn-dark">Reply</button>
            <button v-on:click="ok()" class="card-link btn btn-dark">Ok</button>
          </div>
        </div>
      </li>

      <li>
        <div class="card m-3 border-info" style="width: 18rem;">
          <div class="card-body">
            <h5 class="card-title">amany</h5>
            <h6 class="card-subtitle mb-2 text-muted">1661</h6>
            <p
              class="card-text"
            >{{msg}}GOOD Some quick example text to build the bulk of the card's content.</p>
            <button v-on:click="reply()" class="card-link btn btn-dark">Reply</button>
            <button v-on:click="ok()" class="card-link btn btn-dark">Ok</button>
          </div>
        </div>
      </li>
      <li>
        <div class="card m-3 border-info" style="width: 18rem;">
          <div class="card-body">
            <h5 class="card-title">amany</h5>
            <h6 class="card-subtitle mb-2 text-muted">1661</h6>
            <p
              class="card-text"
            >{{msg}}GOOD Some quick example text to build the bulk of the card's content.</p>
            <button v-on:click="reply()" class="card-link btn btn-dark">Reply</button>
            <button v-on:click="ok()" class="card-link btn btn-dark">Ok</button>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>
y

<script>
export default {
  //  users= [
  //     { name: "amany", msg: "nice website" },
  //     { name: "ahmed", msg: "a helpful app" }
  //   ],
  name: "Message",
  // props: {
  //   // name: String,
  //   // msg: String
  // },
  methods: {
    ok: function() {
      // send ok to client and remove it from the page
      // alert("i have been read it , thanks for your suggestions :)");

      this.$alert("i have been read it , thanks for your suggestions :)");
    },
    reply: function() {
      // alert(
      //   // open a popup to send reply  to client and remove it from the page
      //   "i will disscuss your idea with the owner , thanks for your time sir.."
      // );
      this.$prompt("i will disscuss your idea with the owner , thanks for your time sir..").then(() => {
        //do something...
        console.log("*a*a*a*a*a*");
      });
      
    }
  }
};
</script>

<style scoped>
li {
  display: inline-block;
}
</style>

