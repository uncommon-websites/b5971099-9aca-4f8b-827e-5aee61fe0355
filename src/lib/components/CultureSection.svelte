<script lang="ts">
  const cards = [
    {
      title: "Not Just a Designer...",
      subtitle: "A Strategic Partner.",
      image: "/generated/image-designer-working-at-desk-with-multiple-s-1765655514522-5.webp"
    },
    {
      title: "Not Just Beautiful...",
      subtitle: "Conversion-Focused.",
      image: "/generated/image-close-up-of-hands-typing-on-laptop-with--1765655628954-0.webp"
    },
    {
      title: "Not Just Development...",
      subtitle: "Pixel-Perfect Craft.",
      image: "/generated/image-computer-screen-showing-pixel-perfect-we-1765655631425-1.webp"
    }
  ];
</script>

<section id="about" class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      I'm known for my attention to detail, collaborative approach, and technical expertise. Clients describe me as professional, responsive, and efficient—a true team player who brings both rigor and good humor to every project.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
