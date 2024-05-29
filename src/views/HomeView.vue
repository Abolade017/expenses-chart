<script setup lang="ts">
import BarChart from "@/components/BarChart.vue";
</script>

<template>
  <main class="flex justify-center items-center bg-cream m-48">
    <div class="py-32">
      <div class="bg-orange h-24 rounded-lg mb-6">
        <div class="flex justify-between items-center p-6">
          <div>
            <div class="text-white text-sm">My balance</div>
            <div class="text-white text-lg font-bold pt-2">$921.48</div>
          </div>
          <button>
            <img
              src="/xpense-images/logo.svg"
              alt=" switch-logo"
              class="h-12 w-12"
            />
          </button>
        </div>
      </div>
      <div class="bg-white w-full shadow-md px-6 pt-4 pb-6 rounded-lg">
        <div class="text-lg text-dark-brown font-bold">Spending-Last 7days</div>
        <BarChart class="flex justify-center items-center mb-4"></BarChart>
        <div class="border-t-2 mb-4"></div>
        <div class="flex justify-between items-center">
          <div class="">
            <div class="text-gray-300 text-xs">Total this month</div>
            <div class="text-dark-brown text-2xl font-bold">$478</div>
          </div>
          <div>
            <div class="text-dark-brown text-sm">+2.4%</div>
            <div class="text-gray-300 text-xs">from last month</div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
