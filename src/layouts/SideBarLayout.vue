<script setup lang="ts">
  import FooterView from '@/components/FooterView.vue';
import HelloWorld from '@/components/HelloWorld.vue';
  import SideBarView from '@/components/SideBarView.vue';
</script>

<!-- //////////////////////////////////////////////////////////////////////// -->

<template>
  <div class="two-column-layout">
    <header>
      <SideBarView />
    </header>

    <main>
      <slot />
      <FooterView />
    </main>
  </div>
</template>

<!-- //////////////////////////////////////////////////////////////////////// -->

<style scoped lang="css">
    .two-column-layout {
        display: flex;
        @media (max-width: 768px) {
            flex-direction: column;
        }
    }

    header {
        height: 100vh;
        flex-basis: 20%;
        /* margin-top: 30px; */
    }

    main {
        flex-basis: 80%;
        /* margin-top: 10px; */
        padding: 20px;
    }
</style>
