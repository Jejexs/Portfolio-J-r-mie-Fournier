<template>
    <footer class="columns-2 text-white w-full h-28">
        
        <div class="h-full footertextcenter">
            <NuxtLink to="/mentionslegales" class="footerlink text-2xl" >Mentions légales</NuxtLink>
        </div>


        <div class="h-full footertextcenter">
            <NuxtLink to="/politiquesconfidentialite" class="footerlink text-2xl">Politiques de confidentialité</NuxtLink>
        </div>



    </footer>
</template>

<style>

.footertextcenter{
    display: flex;
  align-items: center;
  justify-content: center;
}

.footerlink {
    background-color: transparent;
    color: #ffffff;
    transition: 0.3s ease-out;
    text-transform: uppercase;
    text-decoration: none;
    display: inline-block;
    padding: 15px 20px;
    position: relative;
  }

  .footerlink:hover:after { 
    width: 100%; 
    left: 0; 
  }

  
  .footerlink:after {    
    background: none repeat scroll 0 0 transparent;
    bottom: 0;
    content: "";
    display: block;
    height: 2px;
    left: 50%;
    position: absolute;
    background: #fff;
    transition: width 0.3s ease 0s, left 0.3s ease 0s;
    width: 0;
  }

</style>