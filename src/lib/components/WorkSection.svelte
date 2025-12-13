<script lang="ts">
  const projects = [
    {
      client: "Easylive.io",
      desc: "Live streaming platform with intuitive UX and modern design.",
      bg: "bg-[#1a1a2e]",
      img: "/generated/image-modern-laptop-screen-showing-a-sleek-liv-1765655499856-0.webp",
      dark: true
    },
    {
      client: "Stellar Coffee",
      desc: "Coffee shop franchise website showcasing locations and brand identity.",
      bg: "bg-[#f4e8d8]",
      img: "/generated/image-warm-coffee-shop-interior-with-modern-br-1765655503540-1.webp",
      dark: false
    },
    {
      client: "VR Arles Festival",
      desc: "Bold and experimental design for a virtual reality arts festival.",
      bg: "bg-[#2a2a3e]",
      img: "/generated/image-person-wearing-vr-headset-in-an-artistic-1765655506679-2.webp",
      dark: true
    },
    {
      client: "Luna for Health",
      desc: "Healthcare platform with clean, accessible design and user journey optimization.",
      bg: "bg-[#e8f4f8]",
      img: "/generated/image-clean-healthcare-app-interface-on-tablet-1765655509115-3.webp",
      dark: false
    },
    {
      client: "Zonama",
      desc: "Modern web presence with strategic content architecture.",
      bg: "bg-[#f0f0f0]",
      img: "https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&q=80&w=800",
      dark: false,
      full: true
    },
    {
      client: "Le Pot au Noir",
      desc: "Restaurant website with immersive visual storytelling.",
      bg: "bg-[#1a1a1a]",
      img: "https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?auto=format&fit=crop&q=80&w=800",
      dark: true
    },
    {
      client: "Orthomaster",
      desc: "Professional healthcare website optimized for conversions.",
      bg: "bg-white",
      img: "/generated/image-professional-dental-or-orthodontic-clini-1765655511734-4.webp",
      dark: false
    }
  ];
</script>

<section id="work" class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-3xl mb-16">
    <h2 class="text-2xl md:text-3xl font-medium leading-tight">
      <span class="font-bold">I craft pixel-perfect Webflow sites</span> that combine strategic UX design with conversion-focused architecture to help French SMBs grow their business online.
    </h2>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-2 gap-x-6 gap-y-12">
    {#each projects as project}
      <div class="group cursor-pointer {project.full ? 'md:col-span-2' : ''}">
        <div class={`aspect-[4/3] w-full rounded-lg overflow-hidden relative ${project.bg} mb-4 ${project.full ? 'md:aspect-[2.5/1]' : ''}`}>
          {#if project.img}
             <img src={project.img} alt={project.client} class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
          {:else}
             <!-- Placeholder for logos on solid bg -->
             <div class="w-full h-full flex items-center justify-center">
                <span class={`text-2xl font-bold ${project.dark ? 'text-white' : 'text-black'}`}>{project.client} Logo</span>
             </div>
          {/if}
        </div>
        <h3 class="text-sm font-bold mb-1">{project.client}</h3>
        <p class="text-sm text-gray-600">{project.desc}</p>
      </div>
    {/each}
  </div>
</section>
