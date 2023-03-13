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
        {
          hid: "og:url",
          property: "og:url",
          content: "https://www.bellpi.com/",
        },
        {
          hid: "og:image",
          property: "og:image",
          content: "https://biz.bellpi.com/logo-bellpi-svg.svg",
        },

        { name: "twitter:card", content: "summary_large_image" },
        {
          hid: "twitter:url",
          name: "twitter:url",
          content: "https://www.bellpi.com/",
        },
        {
          hid: "twitter:title",
          name: "twitter:title",
          content: "Home bonaparte",
        },
        {
          hid: "twitter:image",
          name: "twitter:image",
          content: "https://biz.bellpi.com/logo-bellpi-svg.svg",
        },
      ],
    };
  },
};
</script>
