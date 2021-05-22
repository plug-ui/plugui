<template>
  <docs-page :title="$options.title" :description="$options.description">
    <template #api>
      <docs-properties api-path="/api/loaders.json" />
    </template>
    <docs-card-vue title="CSS Only Loaders" file="examples/loaders/Loaders" />
  </docs-page>
</template>

<script>
import DocsPage from "@/layouts/docs-page.vue";
import DocsProperties from "@/collections/DocsProperties.vue";
import DocsCardVue from "@/collections/docs-card/DocsCardVue.vue";

export default {
  components: {
    DocsCardVue,
    DocsProperties,
    DocsPage,
  },
  title: "CSS Loaders",
  description: `These loaders collection of Plug UI allows the developer to display a lightweight loading animation while doing some time-consuming operation like fetching data etc.`,
};
</script>
