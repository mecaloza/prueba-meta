<template>
  <Tutorial />
</template>

<script>
export default {
  data() {
    return {
      title: "Prueba Esteban",
    };
  },
  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Este es la description",
        },
      ],
    };
  },
};
</script>
