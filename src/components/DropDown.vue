<script lang="ts" setup>

import { ref } from 'vue';

defineProps<{
  title: string,
  items: Array<{
    title: string,
    link: string,
  }>
}>()

const isOpen = ref(false)
const isActive = ref(false)
</script>

<template lang="">
  <div class="navlinks">
    <div class="navlinks-wrapper" @click="isOpen = !isOpen">
      <a
        :class="{ active: isActive }"
        @click="isActive = !isActive"
        class="solutions-navlink-a"
        href="#"
      >
        {{ title }}
      </a>
      <svg
        class="svg"
        width="20"
        height="32"
        viewBox="0 0 448 512"
        :class="{ active: isActive }"
        @click="isActive = !isActive"
      >
        <path
          fill="#3683fc"
          d="M201.4 374.6c12.5 12.5 32.8 12.5 45.3 0l160-160c12.5-12.5 12.5-32.8 0-45.3s-32.8-12.5-45.3 0L224 306.7L86.6 169.4c-12.5-12.5-32.8-12.5-45.3 0s-12.5 32.8 0 45.3l160 160z"
        />
      </svg>
    </div>
    <transition name="fade" appear>
      <div class="dropdown-wrapper" v-if="isOpen">
        <div v-for="(item, i) in items" :key="i">
          <a class="dropdown-item" href="item.link">{{ item.title }}</a>
        </div>
      </div>
    </transition>
  </div>
</template>

<style>
.dropdown-wrapper {
  background-color: #fff;
  display: flex;
  flex-direction: column;
  position: absolute;
  transform: translateX(-3%);
  width: max-content;
  border-radius: 6px;
  margin-top: 1rem;
}

.active.svg {
  transform: rotate(180deg);
}

.dropdown-item {
  text-decoration: none;
  color: #000;
}

.fade-enter-active,
.fade-leave-active {
  transition: all 0.5s ease-out;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}
</style>
