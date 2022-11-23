<script lang="ts" setup>
import { Icon } from "@iconify/vue";
import { computed, ref, watch } from "vue";

const props = defineProps<{
  title: string;
  items: Array<{
    id: number;
    title: string;
    content: string;
  }>;
}>();

const selectedId = ref(0);
const activeChip = computed(() =>
  props.items.filter((x) => x.id === selectedId.value)
);

// watch(activeChip, () => console.log(activeChip.value))
</script>

<template>
  <div>
    <button @click="selectedId = 0" class="solution-navlinks" href="#">
      Depersonalization
    </button>
    <button @click="selectedId = 1" class="solution-navlinks" href="#">
      Prediction
    </button>
    <button @click="selectedId = 2" class="solution-navlinks" href="#">
      Custom Prediction Models
    </button>
    <button @click="selectedId = 3" class="solution-navlinks" href="#">
      Document analysis
    </button>
    <button @click="selectedId = 4" class="solution-navlinks" href="#">
      Data structuring
    </button>
  </div>

  <div class="solution-sections-wrappers">
    <div class="">
      <img src="../assets/Group 4754.png" class="solution-img" />
    </div>
    <div>
      <div>
        <h2>{{ activeChip[0].title }}</h2>
        <p class="solution-section-info">
          {{ activeChip[0].content }}
        </p>
      </div>
      <a class="solutions-learn-more"
        >Learn More
        <Icon
          class="small-icon-learn-more"
          icon="material-symbols:arrow-outward-rounded"
          width="20"
        />
      </a>
    </div>
  </div>
</template>

<style></style>
