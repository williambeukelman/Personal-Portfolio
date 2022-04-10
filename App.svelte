<script>
  import Header from "./components/Header.svelte";
  import Skills from "./components/Skills.svelte";
  import Projects from "./components/Projects.svelte";
  import Education from "./components/Education.svelte";
  import Footer from "./components/Footer.svelte";
</script>

<style>
  main {
    font-family: sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
</style>

<main>
  <!-- Hero Section -->
  <Header/>
  <Skills/>
  <Projects/>
  <Education/>
  <p>Some placeholder content to make the page longer for testing purposes.</p>
  <Footer/>

</main>