<template>
  <div>
    <div v-if="text_first" class="sub-content">
      <div class="sub-content-text">
        <h5 class="c-main-text">
          {{ text }}
        </h5>
      </div>
      <div class="sub-content-illus">
        <slot></slot>
      </div>
    </div>
    <div v-if="!text_first" class="sub-content">
      <div class="sub-content-illus">
        <slot></slot>
      </div>
      <div class="sub-content-text">
        <h5 class="c-main-text">
          {{ text }}
        </h5>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SubContent",
  props: {
    text: String,
    text_first: Boolean,
  },
};
</script>

<style>
.sub-content {
  display: flex;
}

.sub-content-text {
  display: flex;
  margin: 10px;
  max-width: 650px;
}

.sub-content-illus {
  display: flex;
  margin: 20px;
}
</style>