<template>
  <div>
    <div class="content-section introduction">
      <div class="feature-intro">
        <h1>Getting Started</h1>
        <p style="opacity: 0.8">
          PlugUI is the Lightweight &amp; Pluggable CSS only library
        </p>
      </div>
    </div>
    <br />
    <div class="content-section implementation">
      <docs-card title="Installation Guide" :responsive="false">
        <div class="pl-info-msg">
          <i class="light-icon-book"></i>
          <p>Installation docs will be updated soon...</p>
        </div>
      </docs-card>
      <div class="pl-warning-msg pl-shadow__exp-2">
        <i class="light-icon-alert-triangle"></i>
        <p>
          This library is early WIP! Currently the focus is on making PlugUI
          stable and feature complete first.
          <br />
          It is not recommended to use this for anything serious yet.
        </p>
      </div>
      <br />
      <docs-card
        title="Contribution Guide"
        sourceLink="https://github.com/plug-ui/plugui"
        :responsive="false"
      >
        <div class="pl-success-msg">
          <i class="light-icon-brand-github"></i>
          <p>
            Contribution docs will be updated soon...
            <br />
            Meanwhile, feel free to contribute directly on the
            <a
              href="https://github.com/plug-ui/plugui"
              target="_blank"
              class="info-link"
              >GitHub Repository</a
            >
          </p>
        </div>
      </docs-card>
    </div>
  </div>
</template>

<script>
import DocsCard from "@/collections/docs-card/DocsCard.vue";
export default {
  components: {
    DocsCard,
  },
};
</script>

<style lang="scss">
.info-link {
  color: #3e8635;
  font-weight: 600;
  // text-decoration: underline;
}
</style>
