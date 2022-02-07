<template>
  <div class="relative background-gif h-full min-h-screen">
    <div class=" py-10 px-10">
      <a href="http://solanatrollcamp.io" target="_blank" rel="noopener noreferrer">
      <img class="container-gif" src="https://www.solanatrollcamp.io/images/trollgif.gif" style="width: 7vw; height: 13vh" >
      </a>
    </div>
    <div class="pt-10 px-10 flex justify-center align-middle">
      <p class="text-2xl pt-3 px-1 mt-1 text-aqua-1 underline">Welcome Troll</p>
    </div>
     <div class="pt-10 px-10 flex justify-center align-middle">
      <p class="text-sm pt-3 px-2 mt-1 text-aqua ">Here you can stake all your NFT Trolls of Solana Troll Camp </p>
    </div>
      <div class="pt-10 px-10 flex justify-center align-middle">
      <p class="text-sm pt-3 px-2 mt-1 text-aqua ">Please, slect the wallet above, and begin stake </p>
      </div>
    <div class="pt-10 px-10 flex justify-center align-middle">
  
    </div>

    <div class="p-10">
      <router-view />
    </div>

    <div class="pt-10"></div>
  </div>
</template>

<script>
import TheNavBar from '@/components/TheNavBar';
import TheFooter from '@/components/gem-farm/TheFooter';
import TheCat from '@/components/gem-farm/TheCat';
export default {
  components: { TheCat, TheFooter, TheNavBar },
};
</script>

<style>
.container-gif {
  border-width: 7px;
  border-radius: 3px;
}
.background-gif {
  background-image: url("https://i.pinimg.com/originals/cf/ec/88/cfec8819d8376a57c86e3c6e53ed618e.gif");
}
.text-aqua{
   color: rgb(178, 206, 196);
}
.text-aqua-1{
   color: rgb(84, 197, 103);
}
.bg-green{
  background-color: rgb(9, 14, 12);
}
* {
  font-family: 'Press Start 2P', monospace;
}
input[type='radio']:checked + span {
  @apply text-black;
}
</style>
