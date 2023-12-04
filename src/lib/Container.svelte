<script>
  export let testimonial;
  import "../app.css";
  import "../container.css";
</script>

<section
  style={`background-color: ${testimonial.bgColor};`}
  id={testimonial.idName}
>
  {#if testimonial.id === 1}
    <img src="images/bg-pattern-quotation.svg" alt="Quotes" class="quote" />
  {/if}
  <div class="outer-div">
    <img src={testimonial.imageUrl} alt={testimonial.name} class="profile-pic" />
    <div class="inner-div">
      <p
        class={`${testimonial.theme === "dark"
          ? "light-greyish-blue"
          : "dark-blackish-blue"} name`}
      >
        {testimonial.name}
      </p>
      <p
        class={`${testimonial.theme === "dark"
        ? "light-greyish-blue"
        : "dark-blackish-blue"} title`}
      >
        {testimonial.title}
      </p>
    </div>
  </div>
  <p
    class={`${testimonial.theme === "dark"
    ? "light-greyish-blue"
    : "dark-blackish-blue"} heading`}
  >
    {testimonial.heading}
  </p>
  <p
    class={`${testimonial.theme === "dark"
    ? "light-greyish-blue"
    : "dark-blackish-blue"} review`}
  >
    {testimonial.review}
  </p>
</section>
