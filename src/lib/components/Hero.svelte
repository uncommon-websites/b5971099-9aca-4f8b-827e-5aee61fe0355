<script lang="ts">
  // Client logos/names
  const clients = [
    "Easylive",
    "Stellar Coffee",
    "VR Arles Festival",
    "Luna for Health",
    "Orthomaster"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-[#1a1a1a] via-[#2a2a2a] to-white text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#1a1a1a_0%,#2a2a2a_40%,#f5f5f5_70%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Conversion-Focused Webflow Sites That Transform Your Business. <span class="text-gray-500">I help French SMBs turn their online presence into a powerful client acquisition tool through strategic UX design and expert Webflow development.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60">
    <p class="text-xs uppercase tracking-wide text-gray-600">Trusted by</p>
    {#each clients as client}
      <div class="h-8 flex items-center justify-center font-medium text-base text-gray-700">{client}</div>
    {/each}
  </div>
</section>
