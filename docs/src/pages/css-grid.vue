<template>
  <docs-page :title="$options.title" :description="$options.description">
    <template #api>
      <docs-properties api-path="/api/grid.json" />
    </template>
    <docs-card-vue title="Grid" file="examples/grid/Grid" />
    <docs-card-vue title="Auto Width" file="examples/grid/AutoWidth" />
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
  title: "Grid Mechanism",
  description: `The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.`,
};
</script>
