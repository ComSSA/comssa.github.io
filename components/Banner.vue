<template>
  <div class="w-100 banner">
    <a href="https://new.comssa.org.au">
      <span>Click here to see our new website!</span>
      <span>Note: WIP, please give us feedback!</span>
    </a>
  </div>
</template>

<style>
  .banner {
    position: fixed;
    background: #4559A7;
    height: 40px;
    z-index: 1;
  }
  .banner a {
    color: white;
    text-align: center;
    display: flex;
    padding: 2px 0;
    font-size: 12px;
    font-weight: 400;
    flex-direction: column;
    justify-content: center;
  }

  @media (min-width: 576px) {
    .banner a {
      flex-direction: row;
      gap: 10px;
    }
  }
</style>
