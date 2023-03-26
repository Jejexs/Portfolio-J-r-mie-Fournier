<template>
    <a href="#confidentialite">
    <input  type="button" class="inputconfidentialite border-solid text-red-600 rounded-sm border-2 border-red-700 absolute positionbouton text-center" value="Confidentialité" data-cursor="pointer2">
</a>

</template>

<style>

.inputconfidentialite {
    font-size: 2rem;
    padding: 1rem 2rem;
    background-color: transparent;
    color: #ffffff;
    border: 1px solid #393939;
    border-radius: 0;
    box-shadow: 0 0 10px #393939, 0 0 10px #393939 inset;
    text-shadow: 0 0 5px #393939, 0 0 10px #393939;
    transition: 0.3s ease-out;
  }


  .inputconfidentialite:hover {
    color: rgba(255, 255, 255, 0.523);
    background-color: transparent;
    border-color: #393939;
    box-shadow: 0 0 80px #393939;
  }
  
  .inputconfidentialite:active{
    box-shadow: 0 0 30px #393939;
    
  }

</style>

<script>
export default {
  data () {
    return {
      toastIsVisible: false,
      message: '',
      state: ''
    }
  },
  mounted () {
    const cursor = document.querySelector("#cursor");
const cursorBorder = document.querySelector("#cursor-border");
const cursorPos = { x: 0, y: 0 };
const cursorBorderPos = { x: 0, y: 0 };

document.addEventListener("mousemove", (e) => {
  cursorPos.x = e.clientX;
  cursorPos.y = e.clientY;

  cursor.style.transform = `translate(${e.clientX}px, ${e.clientY}px)`;
});

requestAnimationFrame(function loop() {
  const easting = 8;
  cursorBorderPos.x += (cursorPos.x - cursorBorderPos.x) / easting;
  cursorBorderPos.y += (cursorPos.y - cursorBorderPos.y) / easting;

  cursorBorder.style.transform = `translate(${cursorBorderPos.x}px, ${cursorBorderPos.y}px)`;
  requestAnimationFrame(loop);
});

document.querySelectorAll("[data-cursor]").forEach((item) => {
  item.addEventListener("mouseover", (e) => {
    if (item.dataset.cursor === "pointer") {
      cursorBorder.style.backgroundColor = "rgba(255, 255, 255, .6)";
      cursorBorder.style.setProperty("--size", "30px");
    }
    if (item.dataset.cursor === "pointer2") {
      cursorBorder.style.backgroundColor = "white";
      cursorBorder.style.mixBlendMode = "difference";
      cursorBorder.style.setProperty("--size", "80px");
    }
  });
  item.addEventListener("mouseout", (e) => {
    cursorBorder.style.backgroundColor = "unset";
    cursorBorder.style.mixBlendMode = "unset";
    cursorBorder.style.setProperty("--size", "50px");
  });
});

 }
}
</script>