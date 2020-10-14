<template>
  <docs-page :title="$options.title" :description="$options.description">
    <template #api>
      <docs-properties api-path="/api/shadows.json" />
    </template>
    <docs-card-vue title="Box Shadow-1" file="examples/shadow/BoxShadow" />
    <docs-card-vue title="Hover Effect" file="examples/shadow/BoxShadowHover" />
    <docs-card-vue title="Box Shadow-2" file="examples/shadow/BoxShadowExp" />
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
  title: "Box Shadows",
  description: `CSS Buttons Box Layout Module, makes it easier to design flexible
          responsive layout structure without using float or positioning.`,
};
</script>

