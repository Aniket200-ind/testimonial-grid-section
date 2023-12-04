<script>
  export let testimonial;
</script>

<section>
  <div>
    <img src={testimonial.imageUrl} alt={testimonial.name} />
    <p>{testimonial.name}</p>
    <p>{testimonial.title}</p>
  </div>
  <p>
    {testimonial.text}
  </p>
  <p>
    {testimonial.experience}
  </p>
</section>

<style>

</style>
