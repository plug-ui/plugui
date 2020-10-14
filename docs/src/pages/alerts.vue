<template>
  <docs-page :title="$options.title" :description="$options.description">
    <template #api>
      <docs-properties api-path="/api/alerts.json" />
    </template>
    <docs-card-vue title="CSS Alerts" file="examples/warnings/Inline" />
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
  title: "CSS Alerts",
  description: `Inline notifications are used to notify a user of the status of an action during a task flow.`,
};
</script>
