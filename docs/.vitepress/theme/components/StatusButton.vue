<script lang="ts">
export default {
  props: ["link", "text"],
};
</script>

<style>
.status-button {
  display: inline-flex;
}

.status-button button {
  background: orange;
  border-radius: 10px;
  color: var(--primaryBG);
  display: inline;
  font-weight: bold;
  line-height: 30px;
  margin: 14px 4px;
  padding: 0 12px;
}

.status-button button:hover {
  background-color: darkorange;
}
</style>

<template>
  <a :href="link" class="status-button"
    ><button>{{ text }}</button></a
  >
</template>
