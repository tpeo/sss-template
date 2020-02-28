<!-- Svelte Files start with a <script></script> section to define data and functions used by our component (JavaScript!) -->
<script>
  /**
   * To accept parameters for our component, we say:
   *    export let {parameter_name};
   * 
   * To specify a default value if the parameter isn't provided, we say: 
   *    export let {parameter_name} = {default_value};
   * */
  export let title = "Default Title";
  export let description;
</script>

<!-- Svelte Files can also include a <style></style> section to add styles that only apply to this component (CSS / SCSS) -->
<style lang="scss">
  // Using SCSS/SASS, we can import variables and mixins (functions) to our CSS, making it much easier to reuse styles
  @import "./GlobalStyle/theme.scss";

  //Styles that apply to elements with the class="background"
  .background{
    
    //Styles that apply to elements within .background with class="title"
    .title{

    }

    //Styles that apply to elements within .background with class="description"
    .description{

    }

  }
  
</style>

<!-- In addition to the <script></script> and <style></style> sections, we can write our content (HTML) -->
<div class="background">
  <h1 class="title">{title}</h1>
  {#if typeof description !== 'undefined'}
    <h2 class="description">{description}</h2>
  {/if}
</div>