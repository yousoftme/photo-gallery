<template>
  <div id="container">
    <p style="color:white;">
        {{ icon }}
    </p>
    <font-awesome-icon :icon="['fas', icon]" :class="icon + ' alt'"/>
  </div>
</template>

<script setup lang="ts">
defineProps({
  icon: String,
});
</script>

<style scoped>
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 60%;
  transform: translateY(-50%);
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: #8c8c8c;
  margin: 0;
}

</style>
