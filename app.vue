<template>

  
<div class="font-rubik">
  <BaseNav />
  
<NuxtLayout>
  <NuxtPage>
    

  </NuxtPage>
  <Nuxt />
</NuxtLayout>
<div id="cursor"></div>
<div id="cursor-border"></div>
<Retourhaut />
<BaseFooter />
</div>
</template>

<script>
import AOS from 'aos'
import 'aos/dist/aos.css'
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";

import Loader from '~/components/Loader.vue'

gsap.registerPlugin(ScrollTrigger);

export default{

  components: {
    Loader,
  },

  mounted(){

  AOS.init();

    gsap.defaults({ease: "power3"});
gsap.set(".opacityblock", {y: 100});

ScrollTrigger.batch(".opacityblock", {
  //interval: 0.1, // time window (in seconds) for batching to occur. 
  //batchMax: 3,   // maximum batch size (targets)
  onEnter: batch => gsap.to(batch, {autoAlpha: 1, y: 0, stagger: {each: 0.15, grid: [1, 3]}, overwrite: true}),
  onLeave: batch => gsap.set(batch, {autoAlpha: 0, y: -100, overwrite: true}),
  onEnterBack: batch => gsap.to(batch, {autoAlpha: 1, y: 0, stagger: 0.15, overwrite: true}),
  onLeaveBack: batch => gsap.set(batch, {autoAlpha: 0, y: 100, overwrite: true})
  // you can also define things like start, end, etc.
});


// when ScrollTrigger does a refresh(), it maps all the positioning data which 
// factors in transforms, but in this example we're initially setting all the ".box"
// elements to a "y" of 100 solely for the animation in which would throw off the normal 
// positioning, so we use a "refreshInit" listener to reset the y temporarily. When we 
// return a gsap.set() in the listener, it'll automatically revert it after the refresh()!
ScrollTrigger.addEventListener("refreshInit", () => gsap.set(".box", {y: 0}));

  

}



}



</script>

