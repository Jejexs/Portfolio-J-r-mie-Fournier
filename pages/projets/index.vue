<template>
    <div class="bg-gradient-to-b from-blue-500 to-black">
        <div class="w-full h-full">
            
            <img class="gradientbackground" src="../../assets/img/projet.png" alt="">
            <Boutonprojets />
        </div>

        <div id="projets"></div>

            <div>
                <p class="text-6xl text-center pt-20 pb-8 text-white" data-aos="fade-up" data-aos-offset="10" data-aos-delay="100" data-aos-duration="200">DEVELOPPEMENT WEB</p>
            </div>

            <div>
                <p class="text-3xl text-center pt-12 pb-8 text-white" data-aos="fade-up" data-aos-offset="100" data-aos-delay="100" data-aos-duration="200">Coeur d'Agate</p>
            </div>

            <div class="" data-aos="fade-up" data-aos-offset="100" data-aos-delay="100" data-aos-duration="200">
                <div class="content">
                    <a href="https://coeurdagate.com/" target="_blank">
                    <div class="content-overlay"></div>
                    <img class="content-image" src="../../assets/img/coeurdagate.png" alt="">
                    <div class="content-details fadeIn-top">
                        <h3>Coeur d'agate</h3>
                        <p>Coeur d'Agate soutien les aidants et leurs familles en cas de maladie,
                            <br>
                            de vieillissement ou de handicap d'un proche; au travers de manifestations.</p>
                    </div>
                    </a>
                </div>
            </div>

            <div>
                <p class="text-3xl text-center pt-20 pb-8 text-white" data-aos="fade-up" data-aos-offset="50" data-aos-delay="200" data-aos-duration="200">Apopsis Architectes</p>
            </div>

            <div class="" data-aos="fade-up" data-aos-offset="100" data-aos-delay="100" data-aos-duration="200">
                <div class="content">
                    <a href="http://apopsis-architectes.fr/" target="_blank">
                    <div class="content-overlay"></div>
                    <img class="content-image" src="../../assets/img/apopsis.png" alt="">
                    <div class="content-details fadeIn-top">
                        <h3>Apopsis Architectes</h3>
                        <p>Apopsis Architectes est un cabinet d'architecte qui se distingue
                            <br>
                            par sa créativité et son approche novatrice dans la conception et la réalisation de projets architecturaux.</p>
                    </div>
                    </a>
                </div>
            </div>


            <div>
                <p class="text-6xl text-center pt-20 pb-8 text-white" data-aos="fade-up" data-aos-offset="50" data-aos-delay="200" data-aos-duration="200">VIDÉO</p>
            </div>

            <div>
                <p class="text-3xl text-center pt-12 pb-8 text-white" data-aos="fade-up" data-aos-offset="50" data-aos-delay="200" data-aos-duration="200">Trailer Horreur</p>
            </div>

        <div class="blocksproj flex justify-center" data-aos="fade-up" data-aos-offset="100" data-aos-delay="200" data-aos-duration="200">
            <iframe width="60%" height="720px" src="https://www.youtube.com/embed/nzYDLw05zfQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        </div>

        <div>
                <p class="text-3xl text-center pt-12 pb-8 text-white" data-aos="fade-up" data-aos-offset="150" data-aos-delay="200" data-aos-duration="200">Visit My School</p>
            </div>

        <div class="blocksproj flex justify-center pt-6 pb-6" data-aos="fade-up" data-aos-offset="150" data-aos-delay="200" data-aos-duration="200">
            <iframe width="60%" height="720px" src="https://www.youtube.com/embed/_-h3nvwbIIo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
        </div>
        
    </div>
        
    </template>
    
    <style>




.content {
  position: relative;
  width: 70%;
  width: 100%;
  margin: auto;
  overflow: hidden;
}

.content .content-overlay {
  background: rgba(0,0,0,0.7);
  position: absolute;
  height: 100%;
  width: 100%;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  opacity: 0;
  -webkit-transition: all 0.4s ease-in-out 0s;
  -moz-transition: all 0.4s ease-in-out 0s;
  transition: all 0.4s ease-in-out 0s;
}

.content:hover .content-overlay{
  opacity: 1;
}

.content-image{
  width: 100%;
}

.content-details {
  position: absolute;
  text-align: center;
  padding-left: 1em;
  padding-right: 1em;
  width: 100%;
  top: 50%;
  left: 50%;
  opacity: 0;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  -webkit-transition: all 0.3s ease-in-out 0s;
  -moz-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.content:hover .content-details{
  top: 50%;
  left: 50%;
  opacity: 1;
}

.content-details h3{
  color: #fff;
  font-weight: 500;
  letter-spacing: 0.15em;
  margin-bottom: 0.5em;
  text-transform: uppercase;
}

.content-details p{
  color: #fff;
  font-size: 0.8em;
}


.fadeIn-top{
  top: 20%;
}



.divprojet{
    transition-duration: 0.4s;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    
  }

  .blocksproj img{
    min-width: 100%;
    transition: all .3s ease-in-out;
  }

  .blocksproj > div:hover img{
    filter: blur(5px);
  }

  .textImgproj{
   position: absolute;
   z-index: 1000;   
   opacity: 0;
   transition: all .3s ease-in-out;
   font-weight: 300;
   font-size: 65px;
   text-align: center;
   color: black;
   text-shadow: 2px 2px 2px white;
   font-weight: 900;
  }
 
  .blocksproj div{
    transition: all .3s ease-in-out;
  }

  .blocksproj > div:hover p{
    opacity: 1;
  }

  
    
 .gradientbackground{
        -webkit-mask-image: -webkit-gradient(linear, left top, left bottom, 
          from(rgba(0,0,0,1)), to(rgba(0,0,0,0)));
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