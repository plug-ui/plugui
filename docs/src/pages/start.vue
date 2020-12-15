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
        <div class="pl-info-msg ">
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
              <h3>Use the HTML5 doctype</h3>
              <pre><code data-lang="html"><span class="">&lt;!DOCTYPE html&gt;</span></code></pre>
            </div>
            <div class="pl-methods">
              <h3>Use the jsDelivr CDN</h3>
              <a href="https://www.jsdelivr.com/package/npm/plugui"
                >https://www.jsdelivr.com/package/npm/plugui</a
              >
            </div>
            <div class="pl-methods">
              <h3>Download from the repository</h3>
              <a href="https://github.com/plug-ui/plugui"
                >https://github.com/plug-ui/plugui</a
              >
            </div>
            <div class="pl-methods">
              <h3>Starter Template</h3>
              <pre><code class="language-html" data-lang="html"><span class="cp">&lt;!DOCTYPE html&gt;</span>
<span class="">&lt;html&gt;</span>
  <span class="">&lt;head&gt;</span>
    <span class="">&lt;meta</span> <span class="na">charset=</span><span class="">"utf-8"</span><span class="">&gt;</span>
    <span class="">&lt;meta</span> <span class="na">name=</span><span class="">"viewport"</span> <span class="na">content=</span><span class="">"width=device-width, initial-scale=1"</span><span class="">&gt;</span>
    <span class="">&lt;title&gt;</span>Hello Bulma!<span class="">&lt;/title&gt;</span>
    <span class="">&lt;link</span> <span class="na">rel=</span><span class="">"stylesheet"</span> <span class="na">href=</span><span class="">"https://cdn.jsdelivr.net/npm/plugui"</span><span class="">&gt;</span>
  <span class="">&lt;/head&gt;</span>
  <span class="">&lt;body&gt;</span>
  <span class="">&lt;section</span> <span class="na">class=</span><span class="">"section"</span><span class="">&gt;</span>
    <span class="">&lt;div</span> <span class="na">class=</span><span class="">"container"</span><span class="">&gt;</span>
      <span class="">&lt;h1</span> <span class="na">class=</span><span class="">"title"</span><span class="">&gt;</span>
        Hello World
      <span class="">&lt;/h1&gt;</span>
      <span class="">&lt;p</span> <span class="na">class=</span><span class="">"subtitle"</span><span class="">&gt;</span>
        My first website with <span class="">&lt;strong&gt;</span>PLUGUI<span class="">&lt;/strong&gt;</span>!
      <span class="">&lt;/p&gt;</span>
    <span class="">&lt;/div&gt;</span>
  <span class="">&lt;/section&gt;</span>
  <span class="">&lt;/body&gt;</span>
<span class="">&lt;/html&gt;</span></code></pre>
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
        <div class="pl-success-msg">
          <!-- <i class="light-icon-brand-github"></i> -->
          <div class="pl-docs">
            <h3>
              In order to contribute to plugui, you can install its dependencies
              and can preview its docs with hot reload at local host:3000
            </h3>

            PLUG UI is a collection of CSS only Pluggable and Lightweight UI
            Elements
            <h6># Install dependencies</h6>
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
import DocsCard from "@/collections/docs-card/DocsCard.vue";
export default {
  components: {
    DocsCard
  }
};
</script>

<style lang="scss" scoped>
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
  }
  a {
    font-size: 18px;
    font-style: none;
    color: blue;
    font-weight: bold;
  }
  h6 {
    font-size: 16px;
    margin-top: 10px;
  }
}
</style>
