<template>
  <div class="bg-white py-16 px-4 sm:px-6 lg:px-8">
    <div class="max-w-7xl mx-auto">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
        <!-- Left Image -->
        <div class="order-2 lg:order-1 flex items-center justify-center">
          <img
            :src="bgImage"
            alt="Graduate Student in Canada"
            class="rounded-lg shadow-lg w-full h-auto object-cover min-h-[800px]"
          />
        </div>

        <!-- Right Content -->
        <div class="order-1 lg:order-2">
          <h2 class="text-2xl font-bold text-gray-900 mb-6 font-sans">
            Top Universities in Canada
          </h2>
          <ul class="space-y-3 mb-6">
            <li class="text-gray-700 text-lg font-sans">
              University of Toronto
            </li>
            <li class="text-gray-700 text-lg font-sans">
              University of British Columbia (UBC)
            </li>
            <li class="text-gray-700 text-lg font-sans">McGill University</li>
            <li class="text-gray-700 text-lg font-sans">
              University of Alberta
            </li>
            <li class="text-gray-700 text-lg font-sans">
              University of Waterloo
            </li>
          </ul>

          <h2 class="text-2xl font-bold text-gray-900 mb-6 font-sans">
            Popular Courses for Indian Students
          </h2>
          <ul class="space-y-3 mb-6">
            <li class="text-gray-700 text-lg font-sans">
              Business & Management (MBA, Finance, Analytics)
            </li>
            <li class="text-gray-700 text-lg font-sans">
              IT & Computer Science
            </li>
            <li class="text-gray-700 text-lg font-sans">
              Engineering (Computer, Mechanical, Civil, Electrical)
            </li>
            <li class="text-gray-700 text-lg font-sans">
              Health Sciences (Nursing, Public Health, Biotechnology)
            </li>
            <li class="text-gray-700 text-lg font-sans">
              Data Science & Artificial Intelligence
            </li>
          </ul>

          <h2 class="text-2xl font-bold text-gray-900 mb-6 font -sans">
            Scholarships for Indian Students
          </h2>
          <ul class="space-y-3 mb-6">
            <li class="text-gray-700 text-lg">
              <span class="font-semibold text-gray-900 font-sans"
                >Vanier Canada Graduate Scholarships</span
              >
              – Prestigious awards for doctoral students.
            </li>
            <li class="text-gray-700 text-lg">
              <span class="font-semibold text-gray-900 font-sans"
                >Ontario Graduate Scholarship (OGS)</span
              >
              – For students studying in Ontario.
            </li>
            <li class="text-gray-700 text-lg">
              <span class="font-semibold text-gray-900 font-sans"
                >University Entrance & Merit Scholarships</span
              >
              – Offered by institutions like UofT, UBC, and McGill.
            </li>
            <li class="text-gray-700 text-lg">
              <span class="font-semibold text-gray-900 font-sans"
                >Partial Tuition Waivers</span
              >
              – Available for academically strong international students.
            </li>
          </ul>

          <p class="text-gray-600 text-base italic text-lg">
            Tip: Strong IELTS, PTE, or TOEFL scores improve chances of receiving
            scholarships at top Canadian universities.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import bgImage from "@/assets/canada5.png";
</script>

<style scoped></style>
