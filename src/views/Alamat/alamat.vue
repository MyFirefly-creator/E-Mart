<template>
  <Navbar />
  <fieldset class="space-y-3">
    <legend class="sr-only">Delivery</legend>
  
    <div>
      <label
        for="DeliveryStandard"
        class="flex items-center justify-between gap-4 rounded border border-gray-300 bg-white p-3 text-sm font-medium shadow-sm transition-colors hover:bg-gray-50 has-checked:border-blue-600 has-checked:ring-1 has-checked:ring-blue-600 dark:border-gray-600 dark:bg-gray-900 dark:hover:bg-gray-800"
      >
        <div>
          <p class="text-gray-700 dark:text-gray-200">Standard</p>
  
          <p class="text-gray-900 dark:text-white">Free</p>
        </div>
  
        <input
          type="radio"
          name="DeliveryOption"
          value="DeliveryStandard"
          id="DeliveryStandard"
          class="size-5 border-gray-300 dark:border-gray-600 dark:bg-gray-900 dark:ring-offset-gray-900 dark:checked:bg-blue-600"
          checked
        />
      </label>
    </div>
  
    <div>
      <label
        for="DeliveryPriority"
        class="flex items-center justify-between gap-4 rounded border border-gray-300 bg-white p-3 text-sm font-medium shadow-sm transition-colors hover:bg-gray-50 has-checked:border-blue-600 has-checked:ring-1 has-checked:ring-blue-600 dark:border-gray-600 dark:bg-gray-900 dark:hover:bg-gray-800"
      >
        <div>
          <p class="text-gray-700 dark:text-gray-200">Next Day</p>
  
          <p class="text-gray-900 dark:text-white">£9.99</p>
        </div>
  
        <input
          type="radio"
          name="DeliveryOption"
          value="DeliveryPriority"
          id="DeliveryPriority"
          class="size-5 border-gray-300 dark:border-gray-600 dark:bg-gray-900 dark:ring-offset-gray-900 dark:checked:bg-blue-600"
        />
      </label>
    </div>
  </fieldset>
  <a
    class="group relative inline-block text-sm font-medium text-white focus:ring-3 focus:outline-hidden"
    href="create-alamat"
  >
    <span class="absolute inset-0 border border-red-600"></span>
    <span
      class="block border border-red-600 bg-red-600 px-12 py-3 transition-transform group-hover:-translate-x-1 group-hover:-translate-y-1"
    >
      Download
    </span>
  </a>
</template>

<script setup>
import Navbar from '@/components/navbar/navbar.vue';
import { ref, onMounted } from 'vue';
import api from '@/plugins/axios';
</script>