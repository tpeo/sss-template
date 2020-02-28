<script>
  export let seo;
  let { title, rel, description } = seo;
</script>

<svelte:head>
  <title>{title}</title>
  {#if rel}
    <link rel="canonical" href={rel} />
  {/if}
  {#if description}
    <meta name="description" content={description} />
  {:else}
    <meta name="robots" value="noindex, nofollow" />
  {/if}
</svelte:head>
