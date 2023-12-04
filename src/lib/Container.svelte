<script>
  export let testimonial;
  import "../app.css";
  import "../container.css";
</script>

<section
  style={`background-color: ${testimonial.bgColor};`}
  id={testimonial.className}
>
  {#if testimonial.id === 1}
    <img src="images/bg-pattern-quotation.svg" alt="Quotes" id="quote" />
  {/if}
  <div class="outer-div">
    <img src={testimonial.imageUrl} alt={testimonial.name} id="profile-pic" />
    <div id="inner-div">
      <p
        class={testimonial.theme === "dark"
          ? "light-greyish-blue"
          : "dark-blackish-blue"}
        id="name"
      >
        {testimonial.name}
      </p>
      <p
        class={testimonial.theme === "dark"
          ? "light-greyish-blue"
          : "dark-blackish-blue"}
        id="title"
      >
        {testimonial.title}
      </p>
    </div>
  </div>
  <p
    class={testimonial.theme === "dark"
      ? "light-greyish-blue"
      : "dark-blackish-blue"}
    id="heading"
  >
    {testimonial.heading}
  </p>
  <p
    class={testimonial.theme === "dark"
      ? "light-greyish-blue"
      : "dark-blackish-blue"}
    id="review"
  >
    {testimonial.review}
  </p>
</section>