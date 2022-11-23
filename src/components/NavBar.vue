<script lang="ts" setup>
import DropDown from './DropDown.vue';

 const solutions =[
                {
                    title: 'API / Disease pediction',
                    link: '/'
                },
                {
                    title: 'API / Disease Prediction Models',
                    link: '/'
                },
                {
                    title: 'API / Depersonalization',
                    link: '/'
                },
                {
                    title: 'API / Document Analysis',
                    link: '/'
                },
                {
                    title: 'API / Data Structuring',
                    link: '/'
                },
                {
                    title: 'Trials AI simulation',
                    link: '/'
                },
 ]
</script>

<template>
  <div class="header">
    <div class="header-wrapper">
      <div class="logo-wrapper">
        <img class="logo" src="../assets/Logo144.png" />
        <p class="logo-text">
          Longevity <span style="color: #3683fc"> InTime </span> <br />
          Developers
        </p>
      </div>
      <div class="navlinks-wrapper">
        <a class="navlinks" href="#footer">Resources</a>
        <DropDown title="Solutions" :items="solutions" />
        <a class="navlinks" href="#footer">Support</a>
        <a class="navlinks" href="#pricing">Pricing</a>
        <a class="navlinks" href="/">Login</a>
      </div>
    </div>
  </div>
</template>
<style></style>
