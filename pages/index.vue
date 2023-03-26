<template>

<div class="bg-gradient-to-b from-red-800 to-black">

    <div class="w-full h-full ">
      <img class="gradientbackground" src="../img/dev.png" alt="">
      <Boutoncompetences />
    </div>
    <div id="competences">

    </div>

    <div>
      <p class="text-6xl text-center pt-12 text-white" data-aos="fade-up" data-aos-offset="167" data-aos-delay="100" data-aos-duration="200" >COMPÉTENCES</p>

    </div>

    <div class="columns-2 flex justify-center">


        <div class="text-white w-3/4 pt-6 pr-36 pb-6 pl-36" data-aos="fade-up" data-aos-offset="167" data-aos-delay="200" data-aos-duration="200">
          <fieldset style="border: solid white 2px" class="text-4xl pt-6 pb-6 pl-12">
            <legend class="text-xl text-white pr-3 pl-2">LANGAGE DE PROGRAMMATIONtest</legend>
            <ul class="pl-20 pb-2">
              <li>
                HTML
              </li>
              <li>
                CSS
              </li>
              <li>
                JS
              </li>
              <li>
                PHP
              </li>
            </ul>
          </fieldset>

        </div>

        <div class="text-white w-3/4 pt-6 pr-36 pb-6 pl-36" data-aos="fade-up" data-aos-offset="167" data-aos-delay="300" data-aos-duration="200">
          <fieldset style="border: solid white 2px" class="text-4xl pt-6 pb-6 pl-12">
            <legend class="text-xl text-white pr-3 pl-2">FRAMEWORK</legend>
            <ul class="pl-20 pb-2">
              <li>
                Vue.js 
              </li>
              <li>
                Nuxt.js
              </li>
              <li>
                Tailwind CSS
              </li>
              <li>
                
                Symfony
              </li>
            </ul>
          </fieldset>

        </div>


    </div>

    <div class=" flex justify-center w-full" >

        <div class="text-white w-3/4 pt-6 pr-36 pb-6 pl-36" data-aos="fade-up" data-aos-offset="167" data-aos-delay="200" data-aos-duration="200">
            <fieldset style="border: solid white 2px" class="text-3xl pt-6 pb-6 pl-8 columns-2">
                  <legend class="text-xl text-white pl-3 pr-3">COMPÉTENCES SECONDAIRES</legend>
                <p>Montage Vidéo</p>
                <p>Motion Design</p>
                <p>Gestion de projet</p>
                <p>E-Commerce</p>
                <p>Marketing Digital</p>
                <p>Référencement naturel</p>
                <p>Communication</p>
                <p>WordPress</p>
        </fieldset>

        </div>
    </div>

        <div class="flex justify-evenly text-center pt-6 pb-6">
              <div class="image-container" data-aos="fade-up" data-aos-offset="20" data-aos-delay="200" data-aos-duration="200">
                <img src="../assets/img/photoshop.png" alt="Description de l'image">
                <p class="texte-cacher" style="">Photoshop</p>
              </div>
              <div class="image-container" data-aos="fade-up" data-aos-offset="20" data-aos-delay="300" data-aos-duration="200">
                <img src="../assets/img/premierepro.png" alt="Description de l'image">
                <p class="texte-cacher">Premiere Pro</p>
              </div>
              <div class="image-container" data-aos="fade-up" data-aos-offset="20" data-aos-delay="400" data-aos-duration="200">
                <img src="../assets/img/indesign.png" alt="Description de l'image">
                <p class="texte-cacher">InDesign</p>
              </div>
                 
        </div>

        <div class="flex justify-evenly text-center">
              <div class="image-container" data-aos="fade-up" data-aos-offset="20" data-aos-delay="400" data-aos-duration="200">
                <img src="../assets/img/adobexd.png" alt="Description de l'image">
                <p class="texte-cacher" style="">Adobe XD</p>
              </div>
              <div class="image-container" data-aos="fade-up" data-aos-offset="20" data-aos-delay="500" data-aos-duration="200">
                <img src="../assets/img/illustrator.png" alt="Description de l'image">
                <p class="texte-cacher">Illustrator</p>
              </div>
              <div class="image-container" data-aos="fade-up" data-aos-offset="20" data-aos-delay="600" data-aos-duration="200">
                <img src="../assets/img/aftereffects.png" alt="Description de l'image">
                <p class="texte-cacher">After Effects</p>
              </div>
                 
        </div>

        
        

   
    


      <div>
        <p class="text-6xl text-center pt-20 text-white pb-12" data-aos="fade-up" data-aos-offset="80" data-aos-delay="200" data-aos-duration="200">FORMATIONS</p>
      </div>

      <div class="columns-3 text-white  pt-5 pr-5 pl-5 gap-9 blocks">
        <div class="div1" data-aos="fade-up" data-aos-offset="50" data-aos-delay="400" data-aos-duration="200">
          <img src="../assets/img/technicienusinage.png" alt="">
          <p class="textImg">
            Technicien d'usinage
            <br>
            Baccalauréat Professionnel
            <br>
            BAC PRO
          </p>
        </div>

        <div class="div1" data-aos="fade-up" data-aos-offset="50" data-aos-delay="500" data-aos-duration="200">
          <img src="../assets/img/boucher.png" alt="">
          <p class="textImg">
            Boucher
            <br>
            Certificat fédéral de capacité
            <br>
            CFC
          </p>
        </div>

        <div class="div1" data-aos="fade-up" data-aos-offset="50" data-aos-delay="600" data-aos-duration="200">
          <img src="../assets/img/developper.png" alt="">
          <p class="textImg">
            Développeur Web
            <br>
            Bachelor
            <br>
            BAC +3
          </p>
        </div>

        
      </div>

</div>



    
  
</template>
<style>



.opacityblock{
  opacity: 0;
}



.tableaushadow{
  
    box-shadow: 0 0 10px #ffffff, 0 0 10px #ffffff inset;
}


.image-container {
  position: relative;
  width: 150px;
  height: 150px; /* Ajustez cette valeur en fonction de la taille de votre image */
}

.texte-cacher {
  position: absolute;
  top: 50%;
  left: 50%;
  color: white;
  opacity: 0;
  text-align: center;
  transition: opacity 0.5s ease-in-out;
  transform: translate(-50%,-50%);
}

.image-container:hover .texte-cacher {
  opacity: 1;
}

.image-container img {
  width: 100%;
  height: auto;
  transition: opacity 0.5s ease-in-out;
}

.image-container:hover img {
  opacity: 0;
}


</style>

<script>

import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);

export default{

  mounted(){

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


