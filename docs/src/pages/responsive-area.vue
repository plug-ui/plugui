<template>
  <docs-page :title="$options.title" :description="$options.description">
    <template #api>
      <docs-properties api-path="/api/flexbox.json" />
    </template>
    <docs-card-vue
      title="Responsive Area"
      file="collections/docs-card/DocsCard"
    />
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
  title: "Responsive Demo area",
  description: `CSS Buttons Box Layout Module, makes it easier to design flexible
          responsive layout structure without using float or positioning.`,
};
</script>
