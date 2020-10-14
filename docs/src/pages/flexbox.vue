<template>
  <docs-page :title="$options.title" :description="$options.description">
    <template #api>
      <docs-properties api-path="/api/flexbox.json" />
    </template>
    <docs-card-vue
      title="Justify Content"
      file="examples/flex/JustifyContent"
    />
    <docs-card-vue title="Align Items" file="examples/flex/AlignItems" />
    <docs-card-vue title="Align Content" file="examples/flex/AlignContent" />
    <docs-card-vue title="Flex Direction" file="examples/flex/FlexDirection" />
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
  title: "Display Flex",
  description: `CSS Buttons Box Layout Module, makes it easier to design flexible
          responsive layout structure without using float or positioning.`,
};
</script>
