<script lang="ts">
  const testimonials = [
    {
      title: "Sylvain Diaz",
      desc: "\"Nathan demonstrates great competence, listens carefully to client needs, and works with remarkable efficiency and speed.\"",
      img: "/generated/image-happy-small-business-owner-in-their-shop-1765655556465-4.webp"
    },
    {
      title: "Ines Ben Amor",
      desc: "\"His proposals are excellent, he brings rigor to every project, and his good humor makes him a true team player.\"",
      img: "/generated/image-professional-woman-entrepreneur-smiling--1765655558952-5.webp"
    },
    {
      title: "Amina Dilmi",
      desc: "\"Nathan is not just a web designer—he's a digital artist who provides invaluable added value to every project.\"",
      img: "/generated/image-young-female-business-owner-looking-conf-1765655561270-6.webp"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">What clients say about working with me.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      Don't just take my word for it. Here's what clients and collaborators have to say about the experience of working together and the results we've achieved.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each testimonials as testimonial}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={testimonial.img} alt={testimonial.title} class="w-full h-full object-cover grayscale" />
        </div>
        <h4 class="text-xs font-bold mb-1">{testimonial.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{testimonial.desc}</p>
      </div>
    {/each}
  </div>
</section>
