<style scoped>
.contri-list,
.step-3 {
  overflow: hidden;
  position: relative;
}

.step-3 {
  align-content: center;
  align-items: center;
  display: flex;
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
  gap: 24px;
  height: -moz-min-content;
  height: min-content;
  justify-content: flex-start;
  padding: 0;
  width: 100%;
}

.contri-list,
.contri-list-user {
  flex: none;
  transition: all .5s ease;
}

.contri-list {
  height: 40px;
}

.contri-list,
.step-3 {
  overflow: hidden;
  position: relative;
}

.contri-list-user {
  border-radius: 99px;
  bottom: 0;
  left: 0;
  overflow: hidden;
  top: 0;
  width: 40px;
  will-change: transform;
}
</style>

<template>
       <div class="step-3" style="margin-top: 35px;">
        <div class="contri-list" style="display:flex">

          <div v-for="contributor in contributors" :key="contributor.avatar_url" class="contri-list-user">
            <img :src="contributor.avatar_url" alt="Contributor Avatar"
              style="pointer-events:none;user-select:none;display:block;width:100%;height:100%;border-radius:inherit;object-position:center;object-fit:cover;image-rendering:auto">
          </div>

        </div>
      </div>
</template>


<script setup>
const { data: contribuidores } = await useFetch('https://api.github.com/repos/eduhcastro/flutterflow-desktop/contributors')
var contributors = contribuidores.value
</script>