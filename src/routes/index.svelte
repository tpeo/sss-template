<script>
  import Seo from "../components/Seo.svelte";
  import Container from "../components/Container.svelte";
  import Header from "../components/Header.svelte";
  import CTA from "../components/CTA.svelte";
</script>

<style lang="scss">
  @import "../components/GlobalStyle/theme.scss";
</style>

<Seo seo={{
  title: "Svelte + Sapper + SASS Template",
  description: "Template for creating performant websites quickly"
}} />

<!--(TODO) #1: Fill Header with correct parameters -->
<Header />
<!--(TODO) #2: Create Content Component -->
<Container>

</Container>
<!--(TODO) #3: Create Call-To-Action Component -->
<CTA />
