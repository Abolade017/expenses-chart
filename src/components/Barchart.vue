<script setup lang="ts">
import { ref } from "vue";
import { Bar } from "vue-chartjs";
import ChartData from "../assets/data.json";
import {
  Chart as ChartJS,
  Title,
  Tooltip,
  // Legend,
  BarElement,
  CategoryScale,
  LinearScale,
} from "chart.js";

ChartJS.register(
  Title,
  Tooltip,
  // Legend,
  BarElement,
  CategoryScale,
  LinearScale
);
const chartData = ref<any>(ChartData);
const chartOptions = ref({
  responsive: true,
});
</script>

<template>
  <!-- <div class=""> -->
  <Bar id="my-chart-id" :options="chartOptions" :data="chartData" />

  <!-- </div> -->
</template>
