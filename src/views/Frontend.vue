<template>
<main class="container">

  <!-- Inventory System -->
  <project-card code="https://github.com/egle-na/inventorizavimo_sistema" page="https://egle-na.github.io/inventory-system">
    <template v-slot:title>Inventory System</template>
    <template v-slot:description>
      <p>
        Inventory system customized for Teltonika company. Tracking owned, lent, and borrowed gear, get notifications
        when equipment is being lent, returned, or given to you. Easily add or remove equipment. As an admin - add
        and remove users and companies, take ownership of equipment or transfer to other users. It is a single-page
        application developed with the Vue.js framework, vuex, vue-router, Axios, i18n. Backend by: Povilas Tamulis.
      </p>
    </template>
    <template v-slot:display>
      <iframe src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2Fto3EomHM1m5BMdu9AtYEk6%2FInventorius%3Fnode-id%3D0%253A1"
              allowfullscreen
              aria-label="Inventory system design template"
              class="figma-iframe" />
    </template>
  </project-card>

  <!-- Portfolio -->
  <project-card code="https://github.com/egle-na/portfolio" page="/">
    <template v-slot:title>Portfolio Page</template>
    <template v-slot:description>
      <p>
        My custom portfolio page showcasing my work in photography, illustration and frontend development.
        Different image grids and layouts, mobile-first responsive design. Built with Vue.js framework.
      </p>
    </template>
    <template v-slot:display>
      <img src="../assets/images/frontend/Portfolio-screen-capture.jpg" alt="Portfolio page illustrations grid">
    </template>
  </project-card>

  <!-- Maišiagala Kindergarten -->
  <project-card page="https://www.maisiagalosdarzelis.lt/">
    <template v-slot:title>Maišiagala Kindergarten</template>
    <template v-slot:description>
      <p>
        Maišiagala kindergarten website redesign. Currently working on design in Figma. Planing to rebuild
        project using to Vue.js framework. Work in progress.
      </p>
    </template>
    <template v-slot:display>
      <iframe src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2Fyhm6tMPcXpHraV5w6KKVzn%2FDar%25C5%25BEelis%3Fnode-id%3D0%253A1"
              allowfullscreen
              aria-label="Kindergarten design template"
              class="figma-iframe" />
    </template>
  </project-card>

  <!-- GroupIt Extension -->
  <project-card code="https://github.com/egle-na/GroupIt-Extension">
    <template v-slot:title>GroupIt Extension</template>
    <template v-slot:description>
      <p>
        Google Chrome extension that easily stores and opens grouped tabs. It was a fun side project that I made
        for myself to help manage my infinite amount of opened tabs. I did everything from the design in Figma to
        coding and learning about <a href="https://developer.chrome.com/docs/extensions/" rel="nofollow">chrome extensions API</a>.
        Build with simple <abbr title="HyperText Markup Language">HTML</abbr>, <abbr title="Cascading Style Sheets">CSS</abbr> and JavaScript.
      </p>
    </template>
    <template v-slot:display>
<!--   TO DO: change this image   -->
      <img src="../assets/images/frontend/Portfolio-screen-capture.jpg" alt="Portfolio page illustrations grid">
    </template>
  </project-card>

<!--  <project-card>-->
<!--    <template v-slot:title></template>-->
<!--    <template v-slot:description></template>-->
<!--    <template v-slot:button></template>-->
<!--    <template v-slot:display></template>-->
<!--  </project-card>-->

</main>
</template>

<script>
  import ProjectCard from "@/components/ProjectCard";
  export default {
    name: "Frontend",
    components: { ProjectCard },
    mounted() {
      window.scrollTo({
        top: 0,
        bottom: 0,
        behavior: 'smooth'
      });
    }
  }
</script>

<style scoped>

  .figma-iframe {
    border: none;
    width: 100%;
    height: 100%;
    min-height: 300px;
  }
</style>