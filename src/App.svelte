<script>
  import Container from "./lib/Container.svelte";
  import { testimonials } from "./data";
  import "./app.css";
</script>
<main>
  {#each testimonials as testimonial}
    <Container {testimonial} />
  {/each}
</main>