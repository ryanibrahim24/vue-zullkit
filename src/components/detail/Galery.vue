<script setup>
import { ref } from "vue";

const props = defineProps({
  defaultImage: String,
  galleries: Array,
});

const thumbnail = ref(props.defaultImage);

function changeImage(image) {
  this.thumbnail = image;
}
</script>

<template>
  <section id="gallery">
    <img :src="thumbnail" alt="default image" class="w-full mt-6 rounded-2xl" />
    <div class="grid grid-cols-4 gap-4 mt-4">
      <template v-for="galery in galleries" :key="galery.id">
        <div
          @click="changeImage(galery.url)"
          class="overflow-hidden cursor-pointer rounded-2xl"
        >
          <img :src="galery.url" class="w-full" alt="" />
        </div>
      </template>
    </div>
  </section>
</template>
//:class="{ 'ring-2 ring-indigo-500': thumbnail == galery.url }"