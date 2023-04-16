<template>
  <div :style="`width: ${width}; height: ${height}; border-radius: ${round};`" class="skeleton-loader__item"></div>
</template>

<script>
export default {
  name: 'ImpsSkeletonLoader',
  props: {
    width: {
      type: String,
      default: '100%',
    },
    height: {
      type: String,
      default: '5px',
    },
    round: {
      type: String,
      default: '0px',
    }
  },
};
</script>

<style>
  .skeleton-loader__item {
  margin-bottom: 10px;
  background-color: #ddd;
  animation: pulse 1s ease-in-out infinite;
  }

  @keyframes pulse {
  0% {
    opacity: 0.5;
  }
  50% {
    opacity: 1;
  }
  100% {
    opacity: 0.5;
  }
  }
</style>
