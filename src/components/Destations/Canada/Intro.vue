<template>
  <div class="bg-white py-16 px-4 sm:px-6 lg:px-8">
    <div class="max-w-7xl mx-auto">
      <!-- Intro Paragraph - Full Width -->
      <div class="w-full mb-12">
        <p class="text-gray-700 text-lg leading-relaxed font-sans text-lg">
          Canada is one of the most preferred study destinations for
          international students due to its high-quality education system,
          multicultural society, and excellent post-study work opportunities.
          With globally recognized degrees and strong pathways to permanent
          residency, Canada offers students a perfect balance of education and
          career growth.
        </p>
      </div>

      <!-- Image and Content Section -->
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
        <!-- Image Section -->
        <div>
          <img
            :src="bgImage"
            alt="Canadian University Campus"
            class="rounded-lg shadow-lg w-full h-auto object-cover min-h-[500px]"
          />
        </div>

        <!-- Content Section -->
        <div>
          <div class="prose max-w-none">
            <h2 class="text-2xl font-bold text-gray-900 mb-6">
              Why Study in Canada?
            </h2>

            <ul class="space-y-4">
              <li class="text-gray-700 text-lg">
                <span class="font-semibold text-gray-900 font-sans"
                  >World-Class Education</span
                >
                – Canadian universities and colleges are internationally
                recognized for academic excellence and research quality.
              </li>

              <li class="text-gray-700 text-lg">
                <span class="font-semibold text-gray-900 font-sans"
                  >Affordable Study Options</span
                >
                – Tuition fees and living costs are comparatively lower than
                other major study destinations like the USA and UK.
              </li>

              <li class="text-gray-700 text-lg">
                <span class="font-semibold text-gray-900 font-sans"
                  >Post-Graduation Work Permit (PGWP)</span
                >
                – Students can work for up to
                <span class="font-semibold">3 years</span> after completing
                eligible programs.
              </li>

              <li class="text-gray-700 text-lg">
                <span class="font-semibold text-gray-900 font-sans"
                  >Work While Studying</span
                >
                – International students can work up to
                <span class="font-semibold">20 hours per week</span> during
                academic sessions and full-time during breaks.
              </li>

              <li class="text-gray-700 text-lg">
                <span class="font-semibold text-gray-900 font-sans"
                  >PR & Immigration Opportunities</span
                >
                – Canada offers clear pathways to permanent residency through
                programs like Express Entry and Provincial Nominee Programs
                (PNP).
              </li>
            </ul>

            <p class="text-gray-700 text-lg leading-relaxed mt-6 font-sans">
              Graduates in Canada benefit from strong employment prospects in
              fields such as IT, healthcare, engineering, business, and skilled
              trades, supported by a stable economy and inclusive work
              environment.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import bgImage from "@/assets/canada.webp";

// Refs for animation
const introParagraph = ref(null);
const imageSection = ref(null);
const contentSection = ref(null);

let observer = null;

onMounted(() => {
  const options = {
    threshold: 0.15,
    rootMargin: "0px 0px -50px 0px",
  };

  observer = new IntersectionObserver((entries) => {
    entries.forEach((entry) => {
      if (entry.isIntersecting) {
        entry.target.classList.add("is-visible");
      }
    });
  }, options);

  const sections = [
    introParagraph.value,
    imageSection.value,
    contentSection.value,
  ];
  sections.forEach((section) => {
    if (section) observer.observe(section);
  });
});

onUnmounted(() => {
  if (observer) observer.disconnect();
});
</script>

<style scoped></style>
