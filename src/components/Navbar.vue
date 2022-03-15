<template>
  <div id="navbar">
    <header>
      <div
        class="text-white bg-gray-900 py-5 px-10 md:flex md:items-center md:justify-between md:px-40"
      >
        <div class="flex items-center justify-between">
          <div>Logo</div>
          <div class="md:hidden align-middle">
            <i
              class="material-icons align-middle cursor-pointer"
              @click.prevent="toogle"
              >menu</i
            >
          </div>
        </div>
        <div
          :class="open ? 'block' : 'hidden'"
          class="flex flex-col text-left md:block md:text-right mt-3 md:mt-0"
        >
          <a href="#" class="mt-3 md:mx-3">Link 1</a>
          <a href="#" class="mt-3 md:mx-3">Link 2</a>
          <a href="#" class="mt-3 md:mx-3">Link 3</a>
          <a href="#" class="mt-3 md:mx-3">Link 4</a>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: {
    msg: String,
  },
  el: "#navbar",
  data() {
    return {
      open: false,
    };
  },
  methods: {
    toogle() {
      this.open = !this.open;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
