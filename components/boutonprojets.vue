<template>
    <a href="#projets">
    <input  type="button" class="inputprojet border-solid text-blue-500 rounded-sm border-2 border-blue-700 absolute positionbouton text-center" value="Mes projets" data-cursor="pointer2">
</a>

</template>

<style>

.inputprojet {
    font-size: 2rem;
    padding: 1rem 2rem;
    background-color: transparent;
    color: #ffffff;
    border: 1px solid #1e00ff;
    border-radius: 0;
    box-shadow: 0 0 10px #1e00ff, 0 0 10px #1e00ff inset;
    text-shadow: 0 0 5px #1e00ff, 0 0 10px #1e00ff;
    transition: 0.3s ease-out;
  }


  .inputprojet:hover {
    color: rgba(255, 255, 255, 0.523);
    background-color: transparent;
    border-color: #1e00ff;
    box-shadow: 0 0 80px #1e00ff;
  }
  
  .inputprojet:active{
    box-shadow: 0 0 30px #1e00ff;
    
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