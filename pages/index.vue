<template>
  <Tutorial />
</template>

<script>
export default {
  async asyncData({ params }) {
    const data = await fetch(
      "https://admin.bonaparte.com.co/api/v1/product/aacute-rbol-de-levas-cummins-c-1317-5-9l-serie-6bt-ev0210003-49819"
    ).then((res) => res.json());

    console.log("este", data.data.seo);
    return data.data.seo;
  },
  head() {
    var metaTags = this.open_graph.map((tag) => {
      return {
        hid: tag.property,
        name: tag.property,
        content: tag.content,
      };
    });
    metaTags = this.twitter_cards.map((tag) => {
      return {
        hid: tag.name,
        name: tag.name,
        content: tag.content,
      };
    });
    return {
      title: "Este es el titulo",
      meta: metaTags,
    };
  },
};
</script>
