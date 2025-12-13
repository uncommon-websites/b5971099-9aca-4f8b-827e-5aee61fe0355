<script lang="ts">
  const stats = [
    {
      label: "5 Years Experience",
      desc: "With half a decade of expertise in graphic design, web design, and Webflow development, I bring a deep understanding of what makes websites not just beautiful, but effective. Every project benefits from years of refined craft and proven methodologies.",
      icon: "⚡"
    },
    {
      label: "5-Star Ratings",
      desc: "Maintaining perfect 5-star ratings on both Google and Malt platforms speaks to the quality and professionalism I bring to every project. My clients consistently praise my attention to detail, responsiveness, and ability to deliver results that exceed expectations.",
      icon: "⭐"
    },
    {
      label: "Strasbourg, France",
      desc: "Based in the heart of Strasbourg, I serve French SMBs across the country and work with agencies as a white-label partner. My local presence combined with remote capabilities means I can collaborate effectively with clients wherever they are.",
      icon: "📍"
    },
    {
      label: "Webflow Specialist",
      desc: "I specialize in Webflow, a no-code platform with 3.5 million users that offers rapid development, easy evolution, and fast, secure hosting. This expertise allows me to deliver pixel-perfect sites that clients can manage autonomously after launch.",
      icon: "🎯"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white border-t border-gray-100">
  <div class="mb-16">
    <p class="text-gray-500 max-w-xl">
      Curious about my background? Here's a snapshot of my experience, expertise, and what sets me apart.
    </p>
  </div>

  <div class="space-y-16">
    {#each stats as stat}
      <div class="flex flex-col md:flex-row md:items-start justify-between gap-8 border-b border-gray-100 pb-16 last:border-0">
        <h3 class="text-2xl md:text-4xl font-medium w-full md:w-1/3">{stat.label}</h3>
        <div class="w-full md:w-1/3">
           <p class="text-xs leading-relaxed text-gray-500">{stat.desc}</p>
        </div>
        <div class="w-full md:w-1/6 flex justify-end">
           <div class="w-20 h-20 flex items-center justify-center text-4xl bg-gray-50 rounded">{stat.icon}</div>
        </div>
      </div>
    {/each}
  </div>
</section>
