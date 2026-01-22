<template>
  <div class="bg-white py-16 px-4 sm:px-6 lg:px-8">
    <div class="max-w-7xl mx-auto">
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
        <!-- Left Content -->
        <div class="order-2 lg:order-1">
          <h2 class="text-3xl font-bold text-gray-900 mb-6">
            Application & Student Visa Process
          </h2>

          <ul class="space-y-3 mb-6">
            <li class="text-gray-700 text-lg">
              <span class="font-semibold text-gray-900 font-sans">Major Intakes:</span>
              <p>February and July (some universities also offer October).</p>
            </li>
            <li class="text-gray-700 text-lg">
              <span class="font-semibold text-gray-900 font-sans">Requirements:</span>
             <p> English proficiency (IELTS, PTE, TOEFL), academic transcripts,
              SOP, LORs, financial proof. </p>
            </li>
            <li class="text-gray-700 text-lg">
              <span class="font-semibold text-gray-900 font-sans"
                >Student Visa (Subclass 500):</span>
              >
              Requires Confirmation of Enrolment (CoE), Overseas Student Health 
              Cover (OSHC), and proof of funds for tuition + living expenses.
            </li>
          </ul>

          <p class="text-gray-700 text-base leading-relaxed mb-6  text-md font-sans">
            Our team guides students through every step of the Australia student
            visa process in Delhi, ensuring high success rates.
          </p>

          <h2 class="text-3xl font-bold text-gray-900 mb-6 font-sans">
            Why Choose Grace International India for Australia?
          </h2>

          <ul class="space-y-3 mb-6">
            <li class="text-gray-700 text-lg font-sans">
              Direct tie-ups with leading Australian universities.
            </li>
            <li class="text-gray-700 text-base font-sans">
              End-to-end support: counselling, test prep, applications, visas,
              scholarships.
            </li>
            <li class="text-gray-700 text-base font-sans">
              Latest guidance on post-study work and PR pathways.
            </li>
            <li class="text-gray-700 text-base font-sans">
              Pre-departure sessions + on-ground support from Grace offices in
              Australia.
            </li>
            <li class="text-gray-700 text-base font-sans">
              Recognized as one of the best Australia education consultants in
              Delhi with 20+ years of expertise.
            </li>
          </ul>
        </div>

        <!-- Right Image -->
        <div class="order-1 lg:order-2 flex items-center justify-center">
          <img
            :src="australia3"
            alt="Application Process"
            class="rounded-lg shadow-lg w-full h-auto object-cover min-h-[550px]"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import australia3 from "@/assets/australia3.png";
</script>

<style scoped></style>
