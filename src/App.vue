<script>
import Topbar from '@/components/Topbar.vue';
import Sidebar from '@/components/Sidebar.vue';
import Board from '@/components/Board.vue';

export default {
  components: {
    Topbar,
    Sidebar,
    Board
  }
};
</script>

<template>
  <div class="container">
    <header>
      <Topbar />
    </header>
    <main>
      <Sidebar />
      <Board />
    </main>
  </div>  
</template>

<style>
  .container {
    background-color: #f5f5f5;
    display: flex;
    flex-direction: column;
    height: 100vh;
  }

  header {
    background-color: #fff;
    width: 100%;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0px 2px 10px 0px rgba(0,0,0,0.1);
    padding: 15px;
  }

  main {
    padding: 20px;
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: row;
  }

  footer {
    width: 100%;
    display: flex;
    flex-direction: row;
  }
</style>