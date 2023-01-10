<template>
  <div id="frame" class="w-[1920px] h-[1080px] top-20">
    <div id="top" class="h-20 w-full relative">
      <div
        id="title"
        class="w-[900px] absolute h-[110px] flex items-center px-10 overflow-hidden bg-[url(./assets/top_title_bg.svg)]"
        :class="isLight == true ? 'lightBG' : ''">
        <div class="star absolute -left-6 -top-4 animate-[spin_8s_linear_infinite]">
          <svg viewBox="0 0 32 32" class="w-40 h-40">
            <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
              <polygon
                class="fill-red-800"
                fill-rule="nonzero"
                transform="translate(15.695312, 15.695313) rotate(45.000000) translate(-15.695312, -15.695313) "
                points="15.6953115 -6.3046875 20.3690957 6.16143867 21.6894181 9.69310106 25.2210842 11.0134276 37.6953125 15.6953115 25.2291838 20.3690957 21.6975219 21.6894181 20.3771953 25.2210842 15.6953115 37.6953125 11.0215272 25.2291838 9.70120484 21.6975219 6.16953872 20.3771953 -6.3046875 15.6953115 6.16143867 11.0215272 9.69310106 9.70120484 11.0134276 6.16953872"></polygon>
            </g>
          </svg>
        </div>

        <div class="star absolute left-32 -top-2 animate-[spin_4s_linear_infinite]">
          <svg viewBox="0 0 32 32" class="w-20 h-20">
            <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
              <polygon
                class="fill-red-400"
                fill-rule="nonzero"
                transform="translate(15.695312, 15.695313) rotate(45.000000) translate(-15.695312, -15.695313) "
                points="15.6953115 -6.3046875 20.3690957 6.16143867 21.6894181 9.69310106 25.2210842 11.0134276 37.6953125 15.6953115 25.2291838 20.3690957 21.6975219 21.6894181 20.3771953 25.2210842 15.6953115 37.6953125 11.0215272 25.2291838 9.70120484 21.6975219 6.16953872 20.3771953 -6.3046875 15.6953115 6.16143867 11.0215272 9.69310106 9.70120484 11.0134276 6.16953872"></polygon>
            </g>
          </svg>
        </div>

        <div class="star absolute left-64 -bottom-8 animate-[spin_6s_linear_infinite]">
          <svg viewBox="0 0 32 32" class="w-24 h-24">
            <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
              <polygon
                class="fill-red-500"
                fill-rule="nonzero"
                transform="translate(15.695312, 15.695313) rotate(45.000000) translate(-15.695312, -15.695313) "
                points="15.6953115 -6.3046875 20.3690957 6.16143867 21.6894181 9.69310106 25.2210842 11.0134276 37.6953125 15.6953115 25.2291838 20.3690957 21.6975219 21.6894181 20.3771953 25.2210842 15.6953115 37.6953125 11.0215272 25.2291838 9.70120484 21.6975219 6.16953872 20.3771953 -6.3046875 15.6953115 6.16143867 11.0215272 9.69310106 9.70120484 11.0134276 6.16953872"></polygon>
            </g>
          </svg>
        </div>

        <div class="logo relative">
          <svg class="w-20 h-20" viewBox="0 0 1129 1024">
            <path
              d="M234.909 9.656a80.468 80.468 0 0 1 68.398 0 167.374 167.374 0 0 1 41.843 30.578l160.937 140.82h115.07l160.936-140.82a168.983 168.983 0 0 1 41.843-30.578A80.468 80.468 0 0 1 930.96 76.445a80.468 80.468 0 0 1-17.703 53.914 449.818 449.818 0 0 1-35.406 32.187 232.553 232.553 0 0 1-22.531 18.508h100.585a170.593 170.593 0 0 1 118.289 53.109 171.397 171.397 0 0 1 53.914 118.288v462.693a325.897 325.897 0 0 1-4.024 70.007 178.64 178.64 0 0 1-80.468 112.656 173.007 173.007 0 0 1-92.539 25.75h-738.7a341.186 341.186 0 0 1-72.421-4.024A177.835 177.835 0 0 1 28.91 939.065a172.202 172.202 0 0 1-27.36-92.539V388.662a360.498 360.498 0 0 1 0-66.789A177.03 177.03 0 0 1 162.487 178.64h105.414c-16.899-12.07-31.383-26.555-46.672-39.43a80.468 80.468 0 0 1-25.75-65.984 80.468 80.468 0 0 1 39.43-63.57M216.4 321.873a80.468 80.468 0 0 0-63.57 57.937 108.632 108.632 0 0 0 0 30.578v380.615a80.468 80.468 0 0 0 55.523 80.469 106.218 106.218 0 0 0 34.601 5.632h654.208a80.468 80.468 0 0 0 76.444-47.476 112.656 112.656 0 0 0 8.047-53.109v-354.06a135.187 135.187 0 0 0 0-38.625 80.468 80.468 0 0 0-52.304-54.719 129.554 129.554 0 0 0-49.89-7.242H254.22a268.764 268.764 0 0 0-37.82 0z m0 0"
              fill="#fff"></path>
            <path
              d="M348.369 447.404a80.468 80.468 0 0 1 55.523 18.507 80.468 80.468 0 0 1 28.164 59.547v80.468a80.468 80.468 0 0 1-16.094 51.5 80.468 80.468 0 0 1-131.968-9.656 104.609 104.609 0 0 1-10.46-54.719v-80.468a80.468 80.468 0 0 1 70.007-67.593z m416.02 0a80.468 80.468 0 0 1 86.102 75.64v80.468a94.148 94.148 0 0 1-12.07 53.11 80.468 80.468 0 0 1-132.773 0 95.757 95.757 0 0 1-12.875-57.133V519.02a80.468 80.468 0 0 1 70.007-70.812z m0 0"
              fill="#fff"></path>
          </svg>
        </div>

        <div class="text relative text-[50px] text-white ml-10 font-bold">测试标题</div>
      </div>

      <div id="information" class="h-20 bg-black w-full pl-[900px] flex justify-around items-center leading-6">
        <div class="items flex flex-col">
          <span class="text-white">FOLLOW ME</span>
          <span class="text-red-600 font-bold text-xl flex items-center gap-2">
            <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6 fill-red-600" viewBox="0 0 16 16">
              <path
                d="M 11.625 1 C 11.183594 1 10.753906 1.066406 10.351563 1.195313 C 10.085938 1.273438 9.941406 1.554688 10.023438 1.820313 C 10.105469 2.082031 10.382813 2.230469 10.648438 2.148438 C 10.957031 2.050781 11.285156 2 11.625 2 C 13.484375 2 15 3.554688 15 5.5 C 15 5.804688 14.960938 6.101563 14.890625 6.378906 C 14.824219 6.648438 14.988281 6.917969 15.257813 6.984375 C 15.523438 7.050781 15.796875 6.890625 15.863281 6.621094 C 15.953125 6.261719 16 5.886719 16 5.5 C 16 3.027344 14.042969 1 11.625 1 Z M 6.78125 3 C 5.652344 2.980469 3.945313 3.863281 2.429688 5.355469 C 0.917969 6.847656 0.0390625 8.429688 0.0390625 9.796875 C 0.0351563 12.746094 3.441406 14 6.769531 14 C 11.132813 14 14.035156 11.503906 14.035156 9.519531 C 14.035156 8.320313 13.011719 7.640625 12.09375 7.359375 C 11.867188 7.292969 11.710938 7.246094 11.828125 6.953125 C 12.085938 6.320313 12.113281 5.773438 11.832031 5.382813 C 11.3125 4.648438 9.886719 4.6875 8.253906 5.359375 C 8.253906 5.359375 7.738281 5.582031 7.871094 5.179688 C 8.121094 4.386719 8.085938 3.71875 7.695313 3.332031 C 7.472656 3.113281 7.160156 3.007813 6.78125 3 Z M 12 3 C 11.765625 3 11.539063 3.039063 11.328125 3.117188 C 11.15625 3.171875 11.027344 3.316406 10.992188 3.496094 C 10.957031 3.675781 11.023438 3.859375 11.164063 3.976563 C 11.304688 4.09375 11.496094 4.125 11.667969 4.054688 C 11.769531 4.019531 11.878906 4 12 4 C 12.558594 4 13 4.441406 13 5 C 13 5.117188 12.980469 5.230469 12.941406 5.335938 C 12.882813 5.503906 12.917969 5.691406 13.035156 5.828125 C 13.152344 5.964844 13.332031 6.027344 13.507813 5.992188 C 13.683594 5.960938 13.828125 5.835938 13.886719 5.664063 C 13.960938 5.457031 14 5.230469 14 5 C 14 3.902344 13.097656 3 12 3 Z M 6.492188 6.960938 C 8.792969 6.996094 10.878906 7.925781 11.03125 9.429688 C 11.203125 11.148438 9.566406 13 5.625 13 L 5.5 13 C 3.976563 13 2.179688 12.261719 2.007813 10.542969 C 1.832031 8.824219 2.84375 7.257813 5.5 7 C 5.832031 6.96875 6.164063 6.953125 6.492188 6.960938 Z M 5.929688 8.007813 C 4.820313 7.929688 3.6875 8.476563 3.21875 9.351563 C 2.667969 10.375 3.199219 11.511719 4.453125 11.882813 C 5.753906 12.265625 7.285156 11.679688 7.820313 10.574219 C 8.34375 9.496094 7.6875 8.382813 6.402344 8.078125 C 6.246094 8.039063 6.089844 8.019531 5.929688 8.007813 Z M 6.15625 9.351563 C 6.316406 9.40625 6.371094 9.570313 6.285156 9.710938 C 6.195313 9.855469 5.992188 9.925781 5.835938 9.867188 C 5.679688 9.808594 5.628906 9.648438 5.71875 9.507813 C 5.808594 9.367188 6 9.296875 6.15625 9.351563 Z M 4.84375 9.671875 C 4.953125 9.675781 5.0625 9.695313 5.164063 9.734375 C 5.570313 9.890625 5.703125 10.320313 5.453125 10.691406 C 5.199219 11.058594 4.660156 11.222656 4.253906 11.050781 C 3.851563 10.886719 3.734375 10.453125 3.984375 10.09375 C 4.171875 9.828125 4.515625 9.671875 4.84375 9.671875 Z" />
            </svg>
            {{ weibo }}
          </span>
        </div>
        <div class="items flex flex-col">
          <span class="text-white">STREAM CONTENT</span>
          <span class="text-red-600 font-bold text-xl"> Beatmania IIDX, Atelier Series, JRPG </span>
        </div>
      </div>
    </div>

    <main id="main" class="h-[1000px] flex items-center justify-between px-5 bg-[url(./assets/star.svg)]">
      <div id="window" class="h-[900px] w-[1600px] shadow-lg relative border-4 border-red-600">
        <div class="title bg-[url(./assets/window_title_bg.svg)] w-80 h-10 absolute -right-1 -top-11 overflow-hidden">
          <div class="star absolute right-8 animate-[spin_4s_linear_infinite]">
            <svg viewBox="0 0 32 32" class="w-8 h-8">
              <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                <polygon
                  class="fill-red-400"
                  fill-rule="nonzero"
                  transform="translate(15.695312, 15.695313) rotate(45.000000) translate(-15.695312, -15.695313) "
                  points="15.6953115 -6.3046875 20.3690957 6.16143867 21.6894181 9.69310106 25.2210842 11.0134276 37.6953125 15.6953115 25.2291838 20.3690957 21.6975219 21.6894181 20.3771953 25.2210842 15.6953115 37.6953125 11.0215272 25.2291838 9.70120484 21.6975219 6.16953872 20.3771953 -6.3046875 15.6953115 6.16143867 11.0215272 9.69310106 9.70120484 11.0134276 6.16953872"></polygon>
              </g>
            </svg>
          </div>

          <div class="star absolute -right-3 -top-1 animate-[spin_6s_linear_infinite]">
            <svg viewBox="0 0 32 32" class="w-10 h-10">
              <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                <polygon
                  class="fill-red-800"
                  fill-rule="nonzero"
                  transform="translate(15.695312, 15.695313) rotate(45.000000) translate(-15.695312, -15.695313) "
                  points="15.6953115 -6.3046875 20.3690957 6.16143867 21.6894181 9.69310106 25.2210842 11.0134276 37.6953125 15.6953115 25.2291838 20.3690957 21.6975219 21.6894181 20.3771953 25.2210842 15.6953115 37.6953125 11.0215272 25.2291838 9.70120484 21.6975219 6.16953872 20.3771953 -6.3046875 15.6953115 6.16143867 11.0215272 9.69310106 9.70120484 11.0134276 6.16953872"></polygon>
              </g>
            </svg>
          </div>

          <div class="text absolute w-80 h-10 bg-[url(./assets/window_title_text.svg)] bg-no-repeat"></div>
        </div>
      </div>

      <div id="sidebar" class="h-[900px] w-[260px] flex flex-col relative">
        <div class="timing w-full h-10 border-4 text-white text-2xl text-center border-white bg-red-600 shadow-lg absolute -top-10">{{ timing }}</div>

        <div class="chat w-full h-full border-4 border-red-600 mt-6 bg-gradient-to-t via-red-500 from-red-500 to-transparent">
          <h3 class="bg-black text-red-600 font-bold flex text-2xl items-center justify-center h-10">CHATS</h3>
        </div>

        <div class="camera w-full h-[195px] border-4 border-white mt-6">

        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const weibo = ref('@·RCHE·')

let isLight = ref(false)
let timing = ref('')

setInterval(() => {
  console.log(1)
  isLight.value = true
  setTimeout(() => {
    isLight.value = false
  }, 3000)
}, 12000)

const start = new Date()
function timer(start) {
  var now = new Date()
  var det = now - start
  console.log(det)
  now.setTime(det)
  now.setHours(0)
  timing.value = now.toLocaleTimeString()
}

setInterval(() => {
  timer(start)
}, 1000)
</script>

<style scoped>
#frame {
  background: linear-gradient(to top, #020001, #333039, #444a6e, #534d8b);
  background-size: 150% 150%;
  animation: gradientBG 20s ease infinite;
}

#main {
  animation: imgBG 120s linear infinite;
}

#title.lightBG::after {
  content: '';
  position: absolute;
  height: 300px;
  width: 20px;
  background: #fff;
  filter: blur(20px);
  transform: rotate(45deg);
  animation: lightBG 3s linear infinite;
}

@keyframes lightBG {
  0% {
    top: -100px;
    left: -20px;
  }

  100% {
    top: -100px;
    left: 810px;
  }
}

@keyframes imgBG {
  0% {
    background-position: 100% 100%;
  }
  100% {
    background-position: 0% 0%;
  }
}

@keyframes gradientBG {
  0% {
    background-position: 0% 0%;
  }
  50% {
    background-position: 100% 100%;
  }
  100% {
    background-position: 0% 0%;
  }
}
</style>
