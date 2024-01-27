<template>
  <div>
    <Suspense>
      <AsyncCityview />
      <template #fallback>
        <CityViewSkelton />
      </template>
    </Suspense>
  </div>
</template>

<script setup>
import AsyncCityview from "../components/AsyncCityview.vue";
import CityViewSkelton from "@/components/CityViewSkelton.vue";
</script>
