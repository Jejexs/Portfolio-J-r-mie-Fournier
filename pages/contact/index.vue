<template>
    <div class="bg-gradient-to-b from-green-600 to-black">
        <div class="w-full h-full">
            
            <img class="gradientbackground" src="../../assets/img/contact.png" alt="">
            <Boutoncontact />
        </div>
            <div id="contact" class="w-full h-10">

            </div>
       
            <div class="flex justify-center mb-8">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d44235.263098943076!2d6.229625538245209!3d46.1367269032101!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x478c73deeeb249f3%3A0x408ab2ae4ba99e0!2s74930%20Reignier-Esery!5e0!3m2!1sfr!2sfr!4v1678184287907!5m2!1sfr!2sfr" width="60%" height="600" style="border:0;" allowfullscreen="" referrerpolicy="no-referrer-when-downgrade"></iframe>

                
            </div>
            <div class="flex justify-center gap-32 pb-4">

                    <a href="tel:0626144432" data-aos="fade-up" data-aos-offset="20" data-aos-delay="200" data-aos-duration="200" style="background-color: transparent">
                        <div class="flex justify-center flex-col items-center">
                            <img class="h-32 w-32 mb-4 mailtelhover" src="../../assets/img/telephone.png" alt="">
                            <p class="text-white">06 26 14 44 32</p>
                        </div>
                    </a>

                    <a href="mailto:jeremie.fournier@hotmail.com" data-aos="fade-up" data-aos-offset="20" data-aos-delay="300" data-aos-duration="200" style="background-color: transparent">
                        <div class="flex justify-center flex-col items-center boutonmail">
                            <img class="h-32 w-32 mb-4 mailtelhover" src="../../assets/img/mail.png" alt="">
                            <p class="text-white">jeremie.fournier@hotmail.com</p>
                        </div>
                    </a>

                    <a href="/img/JeremieFournierCv.pdf" target="_blank" data-aos="fade-up" data-aos-offset="20" data-aos-delay="400" data-aos-duration="200" style="background-color: transparent">
                        <div class="flex justify-center flex-col items-center">
                            <img class="h-32 w-32 mb-4 mailtelhover" src="../../assets/img/cv.png" alt="">
                            <p class="text-white">Cv PDF</p>
                        </div>
                    </a>

                    <a href="https://www.linkedin.com/in/j%C3%A9r%C3%A9mie-fournier-768729193/" target="_blank" data-aos="fade-up" data-aos-offset="20" data-aos-delay="500" data-aos-duration="200" style="background-color: transparent">
                        <div class="flex justify-center flex-col items-center">
                            <img class="h-32 w-32 mb-4 mailtelhover" src="../../assets/img/linkedin.png" alt="">
                            <p class="text-white">LinkedIn</p>
                        </div>
                    </a>
            </div>

          </div>
        
    </template>
    
    <style>
    
        
    
        .gradientbackground{
        -webkit-mask-image: -webkit-gradient(linear, left top, left bottom, 
          from(rgba(0,0,0,1)), to(rgba(0,0,0,0)));
      }

      .mailtelhover {
  transition: .3s;
    }
    .mailtelhover:hover {
    animation: pulse 1s infinite;
    transition: .3s;
    }
    @keyframes pulse {
    0% {
        transform: scale(1);
    }
    70% {
        transform: scale(.9);
    }
        100% {
        transform: scale(1);
    }
    }
    
    </style>