<template>
    <div class="skeleton-loader">
      <div class="skeleton-loader__item" v-for="n in count" :key="n"></div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'SkeletonLoader',
    props: {
      count: {
        type: Number,
        default: 3,
      },
    },
  };
  </script>
  
  <style>
  .skeleton-loader {
    display: flex;
    flex-direction: column;
  }
  
  .skeleton-loader__item {
    height: 20px;
    width: 100%;
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
  