<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h3>Transfer money to your friends</h3>
    <form>
      <div>
        <label for="">Name</label>
        <input type="text" name="name" id="name">
      </div>
      <div>
        <label for="">Account Number</label>
        <input type="number" name="accountNumber" id="accountNumber">
      </div>
      <div>
        <label for="">Amount</label>
        <input type="number" name="amount" id="amount">
      </div>
      <button>Send</button>
    </form>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator'

@Component
export default class HelloWorld extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
