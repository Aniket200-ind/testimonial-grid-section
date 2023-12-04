<script>
  import Container from "./lib/Container.svelte";
  import { testimonials } from "./data";
</script>
<main>
  {#each testimonials as testimonial}
    <Container {testimonial} />
  {/each}
</main>

<style>
  
</style>
