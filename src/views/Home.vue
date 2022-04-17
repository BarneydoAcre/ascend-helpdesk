<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <SideBar />
    <Ticket />
    <div class="teste">teste</div>
  </div>
</template>

<script>
// @ is an alias to /src
import SideBar from '@/components/SideBar.vue'
import Ticket from '@/components/Ticket.vue'

export default {
  name: 'Home',
  components: {
    SideBar,
    Ticket,
  }
}
</script>

<style>
html, body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  max-width: 100vw;
  max-height: 100vh;
  line-height: 1;
  font-size: 12px;
}
.home {
  width: 100%;
  height: 100%;
  display: grid; 
  grid-template-columns: 60px calc(100vw - 60px);
  grid-template-rows: 100vh;
  grid-template-areas: 
  "sidebar ticket"; 
}
#SideBar {
  grid-area: sidebar;
}
#Ticket {
  grid-area: ticket;
}
</style>
