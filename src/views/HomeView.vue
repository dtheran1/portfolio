<template>
  <main class="flex items-center justify-center min-h-screen text-white" ref="wrapper" @mousemove="moveMouse"
    @mouseleave="mouseLeave">
    <div
      class="rounded-lg border-b border-r p-10 drop-shadow-2xl backdrop-opacity-10 backdrop-invert bg-white/2"
      :style="{ 'transform':`rotateX(${rotationX}deg) rotateY(${rotationY}deg)`}"
      ref="ticket">
      <div class="container">
        <div class="wrapper ">
          <div class="ticket p-10">
            <h1 class="text-7xl font-bold">DANIEL</h1>
            <p class="text-7xl font-bold">THERAN</p>
            <p class="mt-2 transition duration-700 ease-in-out hover:scale-110 cursor-pointer">Frontend Developer</p>
            <div class="bg"></div>
          </div>
        </div>
      </div>
    </div>

  </main>
</template>

<script>
import { ref } from 'vue';


export default {


  // setup() {
  //   const wrapper = ref(null)
  //   const ticket = ref(null)

  //   const rotationX = ref(0)
  //   const rotationY = ref(0)

  //   const moveMouse = (event) => {
  //     const { width, height } = wrapper.value.getBoundingClientRect();
  //     const halfWidth = width / 2;
  //     const halfHeight = height / 2;

  //     const { offsetX, offsetY } = event;
  //     rotationX.value = ((offsetX - halfWidth) / halfWidth) * 20;
  //     rotationY.value = ((offsetY - halfHeight) / halfHeight) * 20;
  //   }

  //   const mouseLeave = () => {
  //     rotationX.value = 0
  //     rotationY.value = 0
  //   }

  //   return { wrapper, moveMouse, ticket, mouseLeave, rotationX, rotationY }
  // }
}

</script>

<style scoped>
.ticket {
  box-shadow: 0 0 40px 5px rgba(0, 0, 0, 0.4);
  width: 600px;
  aspect-ratio: 18/9;
  border-radius: 6px;
  position: relative;
  transition: transform 0.5s ease-in-out;
}

.ticket:hover {
  transition: none;
}

.wrapper {
  perspective: 1000px;
}

.bg {
  top: 0;
  background: rgba(0, 0, 0, 0.3);
  position: absolute;
  filter: blur(20px);
  width: 100%;
  height: 100%;
  z-index: -1;
}

.container {
  display: grid;
}

h1 {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
    Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: white;
  padding: 20px;
}
</style>