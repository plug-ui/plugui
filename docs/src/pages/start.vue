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
        <div class="docs-container">
          <!-- <i class="light-icon-book"></i> -->
          <div class="pl-docs">
            <h4>
              Installing and Using PlugUI is simple and can be done the
              following ways
            </h4>
            <ol>
              <li>Use <b>npm</b> and install the plugui package</li>
              <li>Use our <b>github</b> repository and get the latest</li>
              <li>Use the help of <b>CDN</b></li>
            </ol>
            <div class="pl-methods">
              <h3>Install the plug ui npm package</h3>
              <code-highlight lang="javascript"
                >npm i @plug-ui/plugui</code-highlight
              >
              <code-highlight lang="javascript"
                >//import in css files <br />
                @import "~@plug-ui/plugui/plugui.min.css";
              </code-highlight>
              <code-highlight lang="javascript"
                >//import in JS files
                @import"plug-ui/plugui/plugui.min.css";</code-highlight
              >
              <h3>How to use</h3>
              <code-highlight lang="javascript"
                >import "plug-ui/plugui/plugui.min.css";</code-highlight
              >
            </div>
            <div class="pl-methods">
              <h3>Use the jsDelivr CDN</h3>
              <a
                target="_blank"
                href="https://www.jsdelivr.com/package/npm/@plug-ui/plugui"
                >https://www.jsdelivr.com/package/npm/@plug-ui/plugui</a
              >
            </div>
            <div class="pl-methods">
              <h3>Download from the repository</h3>
              <a target="_blank" href="https://github.com/plug-ui/plugui"
                >https://github.com/plug-ui/plugui</a
              >
            </div>
          </div>
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
        <div class="docs-container">
          <!-- <i class="light-icon-brand-github"></i> -->
          <div class="pl-docs">
            <h3>
              In order to contribute to plugui, you can install its dependencies
              and can preview its docs with hot reload at local host:3000
            </h3>

            PLUG UI is a collection of CSS only Pluggable and Lightweight UI
            Elements, it is currently in version 1.0 with vue/ Nuxt js. The
            actual SCSS files are in the main folder of its Github repository
            and other Docs files are in dosc folder in the Github repository.
            <a target="_blank" href="https://github.com/plug-ui/plugui"
              >Redirect to Github</a
            >
            <h6># Install dependencies</h6>
            <pre><code data-lang="html"><span class="">$ npm install</span></code></pre>
            <pre><code data-lang="html"><span class="">$ npm install</span></code></pre>
            <h6># Preview docs with hot reload at localhost:3000</h6>
            <pre><code data-lang="html"><span class="">$ npm run dev</span></code></pre>
          </div>
        </div>
      </docs-card>
    </div>
  </div>
</template>

<script>
import CodeHighlight from "@/collections/docs-card/CodeHighlight.vue";
import DocsCard from "@/collections/docs-card/DocsCard.vue";
export default {
  components: {
    DocsCard,
    CodeHighlight
  }
};
</script>
<style lang="scss" scoped>
.docs-container {
  padding: 20px;
}
.info-link {
  color: #3e8635;
  font-weight: 600;
  // text-decoration: underline;
}
.pl-docs {
  padding: 10px 0 0 10px;
  display: flex;
  flex-direction: column;
  ol {
    padding: 10px 20px;
    line-height: 2rem;
  }
  h3 {
    color: #333333;
    margin-bottom: 10px;
  }
  .pl-methods {
    margin-bottom: 30px;
  }
  pre {
    display: block;
    width: 100%;
    background-color: #f5f5f5;
    border-radius: 6px;
    color: #586e75;
    padding: 10px;
    margin: 15px 0;
  }
  a {
    font-size: 16px;
    font-style: none;
    color: #39b4ad;
  }
  .inline-links {
    display: flex;
    font-size: 16px;
    font-weight: normal;
    color: #7c7cfa;
    margin-top: 5px;
  }
  h6 {
    font-size: 16px;
    margin-top: 10px;
  }
}
</style>
