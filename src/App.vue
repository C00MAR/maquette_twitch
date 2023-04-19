<script setup>
import TapBar from './view/TapBar.vue'
import ProfilBar from './view/ProfilBar.vue'
import WidthError from './view/WidthError.vue'
import UserOnlineScroll from './view/OnlineUser.vue'
import ClipCard from './components/ClipCard.vue'
import MissBefore from './view/MissBefore.vue'



// Follow me on Twitter & GitHub
// https://twitter.com/sethdavis512
// https://github.com/sethdavis512

// new Vue({
//     el: '#app',
//     data: {
//         window: {
//             width: 0
//         }
//     },
//     created() {
//         window.addEventListener('resize', this.handleResize);
//         this.handleResize();
//     },
//     destroyed() {
//         window.removeEventListener('resize', this.handleResize);
//     },
//     methods: {
//         handleResize() {
//             this.window.width = window.innerWidth;
//         }
//     }
// });



</script>

<template>
  <!-- <WidthError v-if="window.innerWidth < 750"/> -->
  <div class="main">
    <ProfilBar />
    <UserOnlineScroll />
    <ClipCard />
    <MissBefore />
    <ClipCard />
    <TapBar />
  </div>
</template>

<style scoped>
.main{
  display: flex;
  flex-direction: column;
  gap: 3vh;
}
</style>