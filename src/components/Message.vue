<template>
  <div>
    <h1>{{ msg }}</h1>
    <input type="text" v-model="title" />
  </div>
</template>
<script>
export default {
  props: ["msg"],

  data() {
    return {
      title: null
    };
  },
  beforeCreate() {
    console.log("beforeCreate");
  },

  created() {
    console.log("created");
  },

  beforeMount() {
    console.log("beforeMount");
  },

  mounted() {
    console.log("mounted");
  },

  beforeUpdate() {
    console.log("beforeUpdated");
  },

  updated() {
    console.log("updated");
  },

  beforeDestroy() {
    console.log("beforeDelete");
  },

  destroyed() {
    console.log("deleted");
  }
};
</script>
