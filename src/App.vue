<template>
  <div ref="homeFrame" class="w-full h-auto">
    <!-- Desktop/Tablet -->
    <div v-if="!isMobile" class="w=full h-auto bg-[#D5D5D5]">
      <!-- Navbar -->
      <div
        class="fixed top-0 w-full h-[6.25vw] bg-gradient-to-b from-[#D5D5D5] to-transparent backdrop-blur-[1.04vw] px-[8.5vw] flex flex-row justify-between items-center z-30">
        <!-- Left nav -->
        <div class="flex flex-row text-[#1E1E1E]">
          <!-- Logo -->
          <div class="flex flex-col hover:cursor-pointer" @click="scrollToRef('home')">
            <img src="../src/assets/img/Desktop/HomePage/logo.webp" alt="" class="w-[4.6vw] h-auto">
          </div>
          <div class=" flex flex-row items-center text-[#1E1E1E] text-[0.83vw] font-lexend font-bold space-x-[4.58vw]
              pl-[3vw]">
            <p class="hover:cursor-pointer" @click="scrollToRef('home')">Home</p>
            <p class="hover:cursor-pointer" @click="scrollToRef('features')">Features</p>
            <p class="hover:cursor-pointer" @click="scrollToRef('characters')">Characters</p>
            <p class="hover:cursor-pointer" @click="scrollToRef('campaign')">Campaign</p>
            <p class="hover:cursor-pointer" @click="scrollToRef('community')">Community</p>
            <p class="hover:cursor-pointer" @click="scrollToRef('contact')">Contact</p>
          </div>
        </div>
        <!-- Right nav -->
        <div class="relative flex justify-center items-center w-[12.08vw] hover:cursor-pointer button-hover">
          <img src="../src/assets/img/Desktop/HomePage/button.webp" alt="" class="w-full">
          <p class="text-scale text-[#1E1E1E] text-[1.05vw] font-lexend font-bold tracking-[-1.1%] uppercase absolute
             transition-transform duration-300 will-change-transform origin-center">
            Free to play
          </p>
          <div class="overlay-hidden absolute w-[8.9vw] h-[2.083vw] rounded-[50%] bg-[#FFFFFF] mix-blend-overlay blur-[1.85vw]
           opacity-0 transition-opacity duration-300">
          </div>
        </div>
      </div>
      <!-- Content page -->
      <div class="w-full h-auto flex flex-col relative">
        <!-- Section 1 -->
        <div ref="secHome" class="w-full h-[108.64vw] flex relative justify-center">
          <img src="../src/assets/img/Desktop/HomePage/light-golden.webp" alt="" class="absolute top-0 w-full h-auto">
          <img src="../src/assets/img/Desktop/HomePage/pattern.webp" alt=""
            class="absolute top-[-17.1875vw] w-[37.1875vw]">
          <!-- Button middle -->
          <div class="absolute top-[20.5vw] flex flex-col items-center space-y-[1.05vw] w-[33.5vw] z-10">
            <p class="text-center text-[#1E1E1E] text-[3.33vw] font-emeritus tracking-[-1.1%] leading-[3.33vw]">
              An Exciting World of Adventure
            </p>
            <p class="text-center text-[#1E1E1E] text-[0.83vw] font-normal font-lexend">
              Summon your champions to the battlefield of Idle Area! Call forth mighty warriors, upgrade their power,
              and forge an unstoppable team. The fight for glory begins—answer the call now!
            </p>
            <div class="flex justify-center items-center hover:cursor-pointer w-[12.08vw] relative button-hover">
              <img src="../src/assets/img/Desktop/HomePage/button.webp" alt="" class="w-full">
              <p class="text-scale text-[#1E1E1E] text-[1.05vw] font-lexend font-bold tracking-[-1.1%] uppercase absolute
             transition-transform duration-300 will-change-transform origin-center">join now</p>
              <div class="overlay-hidden absolute w-[8.9vw] h-[2.083vw] rounded-[50%] bg-[#FFFFFF] mix-blend-overlay blur-[1.85vw]
           opacity-0 transition-opacity duration-300">
              </div>
            </div>
          </div>
          <!-- images left -->
          <img src="../src/assets/img/Desktop/HomePage/img-left.webp" alt=""
            class="absolute w-[34.5vw] left-[3vw] top-[5.25vw] ">
          <img src="../src/assets/img/Desktop/HomePage/img-right.webp" alt=""
            class="absolute w-[50.625vw] top-[3vw] right-[-2.5vw]">
          <!-- image on bot -->
          <img src="../src/assets/img/Desktop/HomePage/smoke-purple.webp" alt=""
            class="absolute scale-[1.2] top-[72.65625vw]">
          <!-- div after -->
          <div ref="secFeatures" class="absolute top-[52vw] flex flex-col items-center w-full">
            <img src="../src/assets/img/Desktop/HomePage/ball.webp" alt=""
              class="absolute w-[7.4vw] top-[2.86vw] left-[37.7vw]">
            <img src="../src/assets/img/Desktop/HomePage/ball-1.webp" alt=""
              class="absolute w-[4.16vw] top-[12.9vw] left-[30.36vw] z-10">
            <img src="../src/assets/img/Desktop/HomePage/ball-2.webp" alt=""
              class="absolute w-[9.427vw] top-[11.4vw] right-[27.3vw] z-10">
            <img src="../src/assets/img/Desktop/HomePage/cybog.webp" alt="" class="w-[28.7vw] absolute">
            <!-- text -->
            <div class="flex flex-col absolute top-[20.5vw] z-10 items-center space-y-[1.05vw]">
              <p class="text-[#1E1E1E] text-[3.33vw] font-emeritus tracking-[-1.1%] leading-[3.33vw]">Conquer Chapters -
                Climb the Stages
              </p>
              <p class="text-center w-[32.6vw] text-[#1E1E1E] font-lexend text-[0.83vw]">Lead your heroes through an
                epic journey,
                battling enemies and bosses across<br /> countless chapters and stages.</p>
            </div>
            <div class="absolute top-[29.6875vw] w-[83vw] z-10">
              <img src="../src/assets/img/Desktop/HomePage/board.webp" alt="" class="w-full">
            </div>
          </div>
          <img src="../src/assets/img/Desktop/HomePage/light-purple.webp" alt="" class="absolute bottom-0 w-[53.5vw]">
        </div>
        <!-- End Section 1 -->

        <!-- Section 2 -->
        <div class="relative w-full h-[39.6vw] translate-y-[-9vw] flex justify-center items-center">
          <!-- Hon da -->
          <img src="../src/assets/img/Desktop/Experience/smoke-blue.webp" alt=""
            class="w-[22.8125vw] top-[3.5vw] right-[13.8vw] absolute">
          <img src="../src/assets/img/Desktop/Experience/game.webp" alt="" class="w-[32.6vw] h-auto absolute">
          <div class="w-full h-[27vw] bg-gradient-to-b from-[#E8E8E8] to-transparent"
            style="box-shadow: 0vw 0vw 4.16vw 0vw rgba(0,0,0,0.6);">
          </div>
          <div class="absolute top-[7vw] left-[8.5vw] w-[25vw] flex flex-col items-start space-y-[0.78125vw]">
            <p class="text-[#1E1E1E] font-emeritus text-[3.3vw] tracking-[-1.1%] leading-[3.3vw]">
              Experience<br />an exciting
            </p>
            <p class="text-[#F9791C] uppercase font-emeritus text-[4.90625vw] tracking-[-1.1%] leading-[5vw]">Idle RPG
            </p>
            <p class="text-start text-[0.83vw] text-[#1E1E1E] font-lexend">Immerse yourself in a thrilling idle RPG -
              battles never stop.<br />Earn valuable rewards even while you’re offline</p>
          </div>
          <!-- Ruong 1 -->`
          <img src="../src/assets/img/Desktop/Experience/treasure-chest.webp" alt=""
            class="w-[19.375vw] absolute top-[22.875vw] left-[19.32vw]">
          <img src="../src/assets/img/Desktop/Experience/treasure-chest-1.webp" alt=""
            class="w-[14.74vw] absolute left-[12.24vw] top-[25vw]">
          <!-- Reward -->
          <img src="../src/assets/img/Desktop/Experience/reward.webp" alt=""
            class="w-[24.11vw] absolute top-[22.7vw] right-[8.4375vw]">
          <!-- Treasure right 1 -->
          <img src="../src/assets/img/Desktop/Experience/treasure-chest-2.webp" alt=""
            class="w-[9.8vw] absolute top-[33.5vw] right-[11.04vw]">
          <img src="../src/assets/img/Desktop/Experience/treasure-chest-3.webp" alt=""
            class="w-[6.98vw] absolute top-[35.5vw] right-[7.8125vw]">
        </div>
        <!-- End Section 2 -->

        <!-- Section 3 -->
        <div ref="secCampaign" class="relative w-full h-auto flex justify-center pb-[10vw]">
          <!-- Center -->
          <div class="w-[83vw] h-[33.5vw] relative">
            <img src="../src/assets/img/Desktop/Adventure/ADVENTURE_GIRL.webp" alt=""
              class="w-[37vw] absolute top-[-5.3vw] left-[-2vw]">
            <div class="absolute top-[6.35vw] right-0 flex flex-col items-end space-y-[0.78125vw]">
              <p class="text-[#F9791C] text-[5.625vw] font-emeritus uppercase tracking-[-1.1%] leading-[5.625vw]">
                Adventure</p>
              <p class="text-[#1E1E1E] text-[3.33vw] font-emeritus tracking-[-1.1%] leading-[3.33vw]">Conquer all
                challenges</p>
              <p class="text-[#1E1E1E] text-[0.83vw] font-lexend leading-[0.83vw] tracking-[-1.1%]">Immerse yourself in
                a thrilling idle RPG - battles
                never stop.</p>
            </div>
            <!-- Section select -->
            <div class="image-select-list absolute bottom-0 w-full h-[12.08vw] flex">
              <!-- 1 -->
              <div class="thumb smooth-basis h-full relative overflow-hidden rounded-[0.8vw] hover:cursor-pointer"
                :style="growStyle(0)" @click="selectThumb(0)">
                <img :src="adventure1" alt="" class="thumb-img absolute inset-0 w-full h-full object-cover"
                  :style="imgStyle(0)" draggable="false" />
                <div class="abs-ring" :class="ringClass(0)" />
              </div>

              <!-- 2 -->
              <div class="thumb smooth-basis h-full relative overflow-hidden rounded-[0.8vw] hover:cursor-pointer"
                :style="growStyle(1)" @click="selectThumb(1)">
                <img :src="adventure2" alt="" class="thumb-img absolute inset-0 w-full h-full object-cover"
                  :style="imgStyle(1)" draggable="false" />
                <div class="abs-ring" :class="ringClass(1)" />
              </div>

              <!-- 3 -->
              <div class="thumb smooth-basis h-full relative overflow-hidden rounded-[0.8vw] hover:cursor-pointer"
                :style="growStyle(2)" @click="selectThumb(2)">
                <img :src="adventure3" alt="" class="thumb-img absolute inset-0 w-full h-full object-cover"
                  :style="imgStyle(2)" draggable="false" />
                <div class="abs-ring" :class="ringClass(2)" />
              </div>

              <!-- 4 -->
              <div class="thumb smooth-basis h-full relative overflow-hidden rounded-[0.8vw] hover:cursor-pointer"
                :style="growStyle(3)" @click="selectThumb(3)">
                <img :src="adventure4" alt="" class="thumb-img absolute inset-0 w-full h-full object-cover"
                  :style="imgStyle(3)" draggable="false" />
                <div class="abs-ring" :class="ringClass(3)" />
              </div>

              <!-- 5 -->
              <div class="thumb smooth-basis h-full relative overflow-hidden rounded-[0.8vw] hover:cursor-pointer"
                :style="growStyle(4)" @click="selectThumb(4)">
                <img :src="adventure5" alt="" class="thumb-img absolute inset-0 w-full h-full object-cover"
                  :style="imgStyle(4)" draggable="false" />
                <div class="abs-ring" :class="ringClass(4)" />
              </div>
            </div>
          </div>
        </div>
        <!-- End Section 3 -->

        <!-- Section 4 -->
        <div class="relative w-full h-[49.167vw] flex justify-center overflow-hidden">
          <!-- Back convert -->
          <div class="section-1 absolute w-[75vw] h-full left-0 transition-all duration-500 ease-in-out"
            :style="{ background: backGradient }"></div>

          <!-- Circle wheel rotate -->
          <img src="../src/assets/img/Desktop/CHARACTER_WEBP/circle.webp" class="w-[31.25vw] absolute left-[-5vw] bottom-[-9.6vw] origin-center circle-wheel-rotate
         transition-transform duration-500 ease-in-out will-change-transform" :style="wheelStyle" />

          <!-- Text back -->
          <div class="absolute top-[6.64vw] left-[5.2vw] w-[60vw] overflow-hidden">
            <div class="flex will-change-transform transition-transform duration-500 ease-in-out"
              :style="{ transform: `translateX(-${current * 60}vw)` }">
              <p class="text-[17.4vw] w-[60vw] min-w-[60vw] shrink-0 font-emeritus uppercase leading-[15vw]"
                style="background: linear-gradient(180deg, #FFFFFF 0%, #FFB5CB 100%); -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent; color:transparent; opacity:.3;">
                YUMI
              </p>
              <p class="text-[17.4vw] w-[60vw] min-w-[60vw] shrink-0 font-emeritus uppercase leading-[15vw]"
                style="background: linear-gradient(180deg, #FFFFFF 0%, #8ED7FF 100%); -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent; color:transparent; opacity:.3;">
                ZAT
              </p>
              <p class="text-[17.4vw] w-[60vw] min-w-[60vw] shrink-0 font-emeritus uppercase leading-[15vw]"
                style="background: linear-gradient(180deg, #FFFFFF 0%, #FAE36B 100%); -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent; color:transparent; opacity:.3;">
                KONG
              </p>
              <p class="text-[17.4vw] w-[60vw] min-w-[60vw] shrink-0 font-emeritus uppercase leading-[15vw]"
                style="background: linear-gradient(180deg, #FFFFFF 0%, #F06868 100%); -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent; color:transparent; opacity:.3;">
                LUCIAN
              </p>
              <p class="text-[17.4vw] w-[60vw] min-w-[60vw] shrink-0 font-emeritus uppercase leading-[15vw]"
                style="background: linear-gradient(180deg, #FFFFFF 0%, #5CFFC6 100%); -webkit-background-clip:text; background-clip:text; -webkit-text-fill-color:transparent; color:transparent; opacity:.3;">
                KRYSUS
              </p>
            </div>
          </div>

          <!-- Card -->
          <img :src="cardSrc" :style="cardStyle"
            class="absolute pointer-events-none select-none will-change-transform" />

          <!-- Layer -->
          <img src="../src/assets/img/Desktop/CHARACTER_WEBP/layer_backnet.webp" alt=""
            class="h-full absolute bottom-0 right-0">

          <!-- Line color -->
          <div class="w-[36.63vw] absolute top-[20.67vw] left-[25vw]">
            <img src="../src/assets/img/Desktop/CHARACTER_WEBP/nametag.webp" alt="">
            <div class="absolute top-0 left-0 w-[36.63vw]">
              <div class="h-[0.364vw] w-[27.24vw] transition-colors duration-500"
                :style="{ backgroundColor: line1Color }"></div>
            </div>
            <p class="text-[#1e1e1e] text-[3.18vw] font-league font-bold leading-[2.25vw] tracking-[-1.1%]
            absolute bottom-[-0.3vw] left-0">
              {{ slides[current].subtitle }}
            </p>
          </div>

          <!-- Detail -->
          <div class="absolute flex flex-row top-[31.25vw] left-[25vw] space-x-[0.78125vw]">
            <!-- Health -->
            <div class="flex flex-row items-center space-x-[0.3vw]">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/HEART.webp" alt="" class="w-[1.884vw] h-auto">
              <div class="flex flex-col items-start">
                <p class="font-emeritus text-[1.52vw] leading-[1.2vw] tracking-[-1.1%] text-[#1e1e1e]">620</p>
                <p class="font-league text-[#1e1e1e] leading-[1vw] text-[1.12vw]">Health</p>
              </div>
            </div>
            <!-- Attack -->
            <div class="flex flex-row items-center space-x-[0.3vw]">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/ATTACK.webp" alt="" class="w-[1.884vw] h-auto">
              <div class="flex flex-col items-start">
                <p class="font-emeritus text-[1.52vw] leading-[1.2vw] tracking-[-1.1%] text-[#1e1e1e]">78</p>
                <p class="font-league text-[#1e1e1e] leading-[1vw] text-[1.12vw]">Attack</p>
              </div>
            </div>
            <!-- Amor -->
            <div class="flex flex-row items-center space-x-[0.3vw]">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/GUARD.webp" alt="" class="w-[1.884vw] h-auto">
              <div class="flex flex-col items-start">
                <p class="font-emeritus text-[1.52vw] leading-[1.2vw] tracking-[-1.1%] text-[#1e1e1e]">14</p>
                <p class="font-league text-[#1e1e1e] leading-[1vw] text-[1.12vw]">Amor</p>
              </div>
            </div>
          </div>

          <!-- BackCover -->

          <div v-for="(s, i) in slides" :key="`back-${s.key}`"
            class="absolute pointer-events-none will-change-transform actor-slot" :style="backCoverWrapStyleFor(i)"
            :class="backCoverSlotClass(i)">
            <img :src="backCoverMap[s.key].src" :style="[backCoverImgStyleFor(i), revealMaskStyle]"
              class="block select-none pointer-events-none backdrop-blur-[1vw]" draggable="false" />
          </div>

          <!-- blur layer -->
          <div class="absolute w-[8.90625vw] h-[20.98vw] right-[14.43vw] top-[19.0625vw]
         rounded-[50%] blur-[15.625vw] z-10 transition-colors duration-500" :style="{ backgroundColor: glowColor }">
          </div>


          <!-- Rectangle right -->
          <img src="../src/assets/img/Desktop/CHARACTER_WEBP/RectangleVLpng.webp" alt=""
            class="absolute h-[50.5vw] bottom-0 right-[0vw] z-30">

          <!-- Actor -->
          <div class="absolute right-0 top-0 w-[52.08vw] h-[49.167vw] overflow-hidden">
            <div v-for="(s, i) in slides" :key="s.key"
              class="absolute pointer-events-none will-change-transform actor-slot" :style="actorWrapStyleFor(i)"
              :class="actorSlotClass(i)">
              <img :src="actorMap[s.key].src" :style="actorImgStyleFor(i)"
                class="block w-full select-none pointer-events-none" draggable="false" />
            </div>
          </div>

          <!-- Skill -->
          <div class="absolute w-[20vw] top-[26.3vw] left-[25vw] overflow-hidden z-10">
            <div class="flex will-change-transform transition-transform duration-500 ease-in-out"
              :style="{ transform: `translateX(-${current * 20}vw)` }">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/yumiskill.webp" class="w-[20vw] shrink-0">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/zatskills.webp" class="w-[20vw] shrink-0">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/kongyoluwebp.webp" class="w-[20vw] shrink-0">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/zatskill.webp" class="w-[20vw] shrink-0">
              <img src="../src/assets/img/Desktop/CHARACTER_WEBP/krysusskills.webp" class="w-[20vw] shrink-0">
            </div>
          </div>

          <!-- button -->
          <div class="absolute w-[26.58vw] flex justify-between right-[12.54vw] bottom-[4.887vw] z-30">
            <img src="../src/assets/img/Desktop/CHARACTER_WEBP/buttonleft.webp" class="w-[2.72vw] transition"
              :class="canPrev ? 'hover:cursor-pointer' : 'grayscale opacity-50 cursor-not-allowed pointer-events-none'"
              @click="prev" :aria-disabled="!canPrev" />
            <img src="../src/assets/img/Desktop/CHARACTER_WEBP/buttonright.webp" class="w-[2.72vw] transition"
              :class="canNext ? 'hover:cursor-pointer' : 'grayscale opacity-50 cursor-not-allowed pointer-events-none'"
              @click="next" :aria-disabled="!canNext" />
          </div>

          <!-- Score -->
          <img src="../src/assets/img/Desktop/CHARACTER_WEBP/level.webp" alt=""
            class="w-[11.3vw] absolute top-[34.375vw] left-[25vw]">
        </div>
        <!-- End Section 4 -->

        <!-- Section 5 -->
        <div ref="secCharacters" class="relative w-full h-[104.6vw] flex justify-center overflow-hidden bg-[#fffcec]">
          <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Backdrop_1.webp" alt="" class="w-full h-auto absolute top-0">
          <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Yellow_Wheel.webp" alt=""
            class="w-[42.5vw] absolute top-[-8.1vw] right-[-18vw]">
          <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Xinzhao.webp" alt=""
            class="w-[35.46875vw] absolute top-[9.16666vw] right-[6.40625vw]">
          <!-- AWAKEN EMBER -->
          <div class="absolute w-[54.74vw] h-auto top-[12.76vw] left-[9.79vw]">
            <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Awaken_Ember.webp" alt="" class="w-full h-auto">
            <p class="absolute text-[#1E1E1E] font-emeritus text-[2.36vw] top-0 tracking-[-1.1%]">Awaken Ember</p>
            <p
              class="absolute text-[#1E1E1E] font-league text-[0.9375vw] tracking-[-1.1%] top-[3.54vw] w-[49.32vw] leading-[1.32vw]">
              Description: This group of characters carries within them a mysterious, primal energy, awakened from a
              forgotten world. The characters in Awaken Ember possess ancient powers and the ability to control fire
              or
              natural elements. They are not only powerful but also exude an aura of mysticism, inspired by ancient
              creatures and arcane magic.
              <br />
              Key Features:
              <br />
              • Supernatural powers derived from fire or natural elements.
              <br />
              • Ability to heal quickly thanks to mystical energy.
              <br />
              • Can summon creatures or natural elements to assist in combat.
            </p>
          </div>

          <!-- BEAST -->
          <div class="absolute w-[57.1875vw] top-[29.01vw] left-[5.2vw]">
            <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Beast.webp" alt="" class="w-full">
            <p class="absolute text-[#1E1E1E] font-emeritus text-[2.36vw] top-0 tracking-[-1.1%]">Beast</p>
            <p
              class="absolute text-[#1E1E1E] font-league text-[0.9375vw] tracking-[-1.1%] top-[3.54vw] w-[49.32vw] leading-[1.32vw]">
              Description: The warriors in the Beast group possess extraordinary strength, derived from their wild
              instincts and powerful physiques. They are inspired by fierce beasts, embodying unmatched strength and
              primal combat prowess. Their battle style is aggressive and relentless, never hesitating to charge into
              battle with full force.
              <br />
              Key Features:
              <br />
              • Exceptional physical strength and speed.
              <br />
              • Powerful close-range combat abilities with devastating attacks.
              <br />
              • Special expertise in using heavy weapons or combat techniques tied to nature.
            </p>
          </div>

          <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Back2.webp" alt="" class="absolute bottom-0 right-0">
          <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Blue_Wheel.webp" alt=""
            class="w-[43.54vw] absolute top-[39.0625vw] left-[-19.53125vw]">
          <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Kathus.webp" alt=""
            class="w-[27.083vw] absolute top-[57.7vw] left-[6vw]">

          <!-- Cyborg -->
          <div class="absolute top-[50.99vw] w-[56.40625vw] right-[10.99vw]">
            <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Cyborg.webp" alt="" class="w-full h-auto">
            <p class="absolute text-[#1E1E1E] font-emeritus text-[2.36vw] top-0 tracking-[-1.1%]">Cyborg</p>
            <p
              class="absolute text-[#1E1E1E] font-league text-[0.9375vw] tracking-[-1.1%] top-[3.54vw] w-[49.32vw] leading-[1.32vw]">
              Description: The Cyborg group is a fusion of man and machine, where warriors are enhanced with advanced
              technology. These characters have mechanical body parts that significantly boost their physical strength
              and combat abilities. They also possess the ability to control machinery and harness cutting-edge
              technology in battle.
              <br />
              Key Features:
              <br />
              • A combination of human body and robotic parts, enhancing strength and speed.
              <br />
              • Capable of using advanced technology and controlling devices remotely.
              <br />
              • Highly durable in long battles, with quick self-repair abilities thanks to technology.
            </p>
          </div>

          <!-- Human -->
          <div class="absolute top-[67.7vw] w-[56.40625vw] right-[3.229vw]">
            <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Human.webp" alt="" class="w-full h-auto">
            <p class="absolute text-[#1E1E1E] font-emeritus text-[2.36vw] top-0 tracking-[-1.1%]">Human</p>
            <p
              class="absolute text-[#1E1E1E] font-league text-[0.9375vw] tracking-[-1.1%] top-[4vw] w-[51vw] leading-[1.5vw]">
              Description: This group consists of human warriors who possess special abilities without relying on
              technology or magic. These characters are flexible and skilled, ranging from experienced fighters to
              expert explorers. They excel in combat through strategy, dexterity, and adaptability in tough
              situations.
              <br />
              Key Features:
              <br />
              • Diverse combat skills and tactics.
              <br />
              • High flexibility, able to use a wide range of weapons and gear.
              <br />
              • Resilience and the ability to adapt to any battlefield.
            </p>
          </div>

          <!-- Ultron -->
          <div class="absolute top-[84.43vw] left-[40vw] w-[56vw]">
            <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Ultron.webp" alt="" class="w-full h-auto">
            <p class="absolute text-[#1E1E1E] font-emeritus text-[2.36vw] top-0 tracking-[-1.1%]">Ultron</p>
            <p
              class="absolute text-[#1E1E1E] font-league text-[0.9375vw] tracking-[-1.1%] top-[3.54vw] w-[49.32vw] leading-[1.4vw]">
              Description: The Ultron group features characters with superior technological abilities, blending
              artificial intelligence with enhanced strength. They have intelligent minds and systems capable of
              analyzing and predicting battles instantly. The characters in the Ultron group can create powerful
              weapons
              and maintain constant offensive capabilities.
              <br />
              Key Features:
              <br />
              • Possess artificial intelligence and the ability to optimize combat strategies.
              <br />
              • Can control high-tech weapons and create support tools for combat.
              <br />
              • Consistent strength and the ability to battle with superior capabilities, always staying one step
              ahead
              of the enemy.
            </p>
          </div>
        </div>
        <!-- End Section 5 -->

        <!-- Section 6 -->
        <div class="relative w-full h-auto flex overflow-hidden flex-col items-center bg-[#fffcec]">
          <div ref="secContact" class="relative w-full h-[47vw] flex justify-center">
            <img src="../src/assets/img/Desktop/CTA/CTA_Wheel_back.webp" alt=""
              class="w-[45.1vw] absolute top-[6.615vw]">
            <img src="../src/assets/img/Desktop/CTA/CTA_Darius.webp" alt="" class="w-[40.416vw] absolute top-[10vw]">
            <!-- Text left -->
            <div class="absolute w-[25.88vw] top-[18.646vw] left-[5.2vw] space-y-[1vw]">
              <p class="text-[#1E1E1E] text-[2.083vw] font-emeritus text-start tracking-[-1.1%] leading-[2.25vw]">
                Kickstart Your Adventure in Style
              </p>
              <p class="text-[#1E1E1E] text-[0.83vw] font-league text-start tracking-[-1.1%] leading-[1.2vw]">Log in
                for
                the first time to claim valuable gifts and
                limited-time bonuses!
                Boost your
                journey, unlock exclusive gear, and start your gaming adventure with excitement.</p>
              <div
                class="w-[12.083vw] flex relative items-center justify-center ml-[5vw] hover:cursor-pointer button-hover">
                <img src="../src/assets/img/Desktop/HomePage/button.webp" alt="" class="w-full h-auto">
                <p class="text-scale text-[#1E1E1E] text-[1.05vw] font-lexend font-bold tracking-[-1.1%] uppercase absolute
             transition-transform duration-300 will-change-transform origin-center">
                  Free to play
                </p>
                <div class="overlay-hidden absolute w-[8.9vw] h-[2.083vw] rounded-[50%] bg-[#FFFFFF] mix-blend-overlay blur-[1.85vw]
           opacity-0 transition-opacity duration-300">
                </div>
              </div>
            </div>

            <!-- Text Right -->
            <div
              class="absolute flex flex-col items-center w-[24.84375vw] top-[18.636vw] right-[5.2vw] space-y-[1.05vw]">
              <p class="text-[#1E1E1E] text-[2.083vw] font-emeritus leading-[2.1vw]">
                Play Now – Anywhere!
              </p>
              <div class="flex flex-row space-x-[1.1vw]">
                <!-- Button App Store -->
                <div
                  class="w-[9.375vw] h-[2.708vw] rounded-[0.4vw] border-[1px] border-[#A6A6A6] bg-white flex flex-row items-center justify-center space-x-[0.5vw] hover:cursor-pointer">
                  <img src="../src/assets/img/Desktop/CTA/CTA_Apple.webp" alt="" class="w-[1.44vw] h-[1.73vw]">
                  <img src="../src/assets/img/Desktop/CTA/AppStore.png" alt="" class="w-[5.52vw]">
                </div>
                <!-- Button Google Play -->
                <div
                  class="w-[9.375vw] h-[2.708vw] rounded-[0.4vw] border-[1px] border-[#A6A6A6] bg-white flex flex-row items-center justify-center space-x-[0.5vw] hover:cursor-pointer">
                  <img src="../src/assets/img/Desktop/CTA/CTA_GG_Play.webp" alt="" class="w-[1.6vw] h-[1.74vw]">
                  <img src="../src/assets/img/Desktop/CTA/GGPLay.png" alt="" class="w-[5.8875vw]">
                </div>
              </div>
            </div>

            <!-- Div end -->
            <div class="absolute bottom-0 w-full h-[11.09vw] overflow-hidden">
              <!-- Back -->
              <div class="absolute bottom-0 h-[7.39vw] w-full flex flex-row justify-start">
                <img src="../src/assets/img/Desktop/CTA/CTA_Discord_Back.webp" alt=""
                  class="h-[7.39vw] w-[54.53125vw] absolute left-0 bottom-0">
                <img src="../src/assets/img/Desktop/CTA/CTA_Facebook_Back.webp" alt=""
                  class="h-[7.39vw] w-[54.53125vw] absolute right-0 bottom-0">
              </div>
              <!-- Shark -->
              <img src="../src/assets/img/Desktop/CTA/CTA_Discord_CaSau.webp" alt=""
                class="w-[16.51vw] absolute bottom-0 left-[2.5vw]">
              <!-- Logo Discord -->
              <div
                class="x left-[23vw] absolute bottom-[2vw] flex flex-row items-center space-x-[0.6vw] hover:cursor-pointer hover:scale-[1.1] origin-center transition-transform duration-300">
                <img src="../src/assets/img/Desktop/CTA/Telegram2.png" alt="" class=" w-[3vw]">
                <div class="flex flex-col items-start h-[2.8vw] justify-between">
                  <p class="text-[#FFF] text-[1.2vw] font-league leading-[1.2vw] font-bold">
                    Join us on
                  </p>
                  <p class="text-[#FFF] text-[2.4vw] font-emeritus leading-[2.4vw] translate-y-[-0.3vw]">Twitter</p>
                </div>
              </div>
              <!-- Blitcrank -->
              <img src="../src/assets/img/Desktop/CTA/CTA_Facebook_Blitzcrank.webp" alt=""
                class="w-[11.61vw] absolute right-[2.343675vw] bottom-[-1vw]">
              <!-- Logo Facebook -->
              <div
                class="tele w-[12.45vw] absolute bottom-[1.7vw] right-[24vw] flex flex-row items-center hover:cursor-pointer hover:scale-[1.1] origin-center transition-transform duration-300 space-x-[0.6vw]">
                <img src="../src/assets/img/Desktop/CTA/TelegramBlue.png" alt="" class="hover:cursor-pointer w-[3.6vw]">
                <p class="text-[2.4vw] font-emeritus text-white" style="text-shadow: 0 0.05vw 0.3vw #ccc;">Telegram</p>
              </div>
            </div>
          </div>

          <!-- Community -->
          <div ref="secCommunity" class="relative w-full flex flex-col items-center">
            <img src="../src/assets/img/Desktop/CTA/CTA_Back.webp" alt="" class="w-full h-auto" />
            <img src="../src/assets/img/Desktop/CTA/CTA_O_tren.webp" alt="" class="w-full h-auto absolute top-0" />
            <img src="../src/assets/img/Desktop/CTA/CTA_Man_Last.webp" alt=""
              class="w-[46vw] absolute top-[11.7vw] right-[1vw]">
            <p
              class="text-[5.3078125vw] font-emeritus uppercase absolute leading-[5vw] bottom-[3.2vw] bg-gradient-to-b from-[#555A7C] to-[#0F1016] bg-clip-text text-transparent">
              COMMUNITY</p>
            <img src="../src/assets/img/Desktop/CTA/CTA_O_duoi.webp" alt="" class="w-full h-auto absolute bottom-0" />

            <!-- Feedback -->
            <div class="w-[45vw] h-[25.68vw] flex flex-col justify-between absolute top-[8.3vw] left-[5.2vw]">
              <!-- Row 1 -->
              <div class="flex flex-row justify-between">
                <!-- Div 1 -->
                <div class="w-[22vw] relative">
                  <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
                  <!-- FEEDBACK 1 -->
                  <div class="absolute top-[2.08vw] left-[1.146vw] flex flex-col items-start">
                    <!-- name -->
                    <div class="flex flex-row space-x-[0.625vw] items-center">
                      <p class="text-[#1E1E1E] font-emeritus tracking-[-1.1%] text-[1.25vw] leading-[1.35vw]">Jake M
                      </p>
                      <div class="flex flex-row space-x-[0.1vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                      </div>
                    </div>
                    <!-- Detail -->
                    <div
                      class="w-[17.19vw] h-auto text-[0.9375vw] text-[#1E1E1E] font-league leading-[1.40625vw] text-start">
                      “Idle Arena is super chill and addictive. Perfect for quick breaks!”
                    </div>
                  </div>
                </div>
                <!-- Div 2 -->
                <div class="w-[22vw] relative">
                  <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
                  <!-- FEEDBACK 1 -->
                  <div class="absolute top-[2.08vw] left-[1.146vw] flex flex-col items-start">
                    <!-- name -->
                    <div class="flex flex-row space-x-[0.625vw] items-center">
                      <p class="text-[#1E1E1E] font-emeritus tracking-[-1.1%] text-[1.25vw] leading-[1.35vw]">Emily R
                      </p>
                      <div class="flex flex-row space-x-[0.1vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                      </div>
                    </div>
                    <!-- Detail -->
                    <div
                      class="w-[17.19vw] h-auto text-[0.9375vw] text-[#1E1E1E] font-league leading-[1.40625vw] text-start">
                      “Love the graphics and easy gameplay. Great way to kill time.”
                    </div>
                  </div>
                </div>
              </div>

              <!-- Row 2 -->
              <div class="flex flex-row justify-between">
                <!-- Div 1 -->
                <div class="w-[22vw] relative">
                  <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
                  <!-- FEEDBACK 1 -->
                  <div class="absolute top-[2.08vw] left-[1.146vw] flex flex-col items-start">
                    <!-- name -->
                    <div class="flex flex-row space-x-[0.625vw] items-center">
                      <p class="text-[#1E1E1E] font-emeritus tracking-[-1.1%] text-[1.25vw] leading-[1.35vw]">Noah T
                      </p>
                      <div class="flex flex-row space-x-[0.1vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                      </div>
                    </div>
                    <!-- Detail -->
                    <div
                      class="w-[17.19vw] h-auto text-[0.9375vw] text-[#1E1E1E] font-league leading-[1.40625vw] text-start">
                      “Perfect for casual gaming. Easy to pick up, hard to put down.”
                    </div>
                  </div>
                </div>
                <!-- Div 2 -->
                <div class="w-[22vw] relative">
                  <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
                  <!-- FEEDBACK 1 -->
                  <div class="absolute top-[2.08vw] left-[1.146vw] flex flex-col items-start">
                    <!-- name -->
                    <div class="flex flex-row space-x-[0.625vw] items-center">
                      <p class="text-[#1E1E1E] font-emeritus tracking-[-1.1%] text-[1.25vw] leading-[1.35vw]">Liam S
                      </p>
                      <div class="flex flex-row space-x-[0.1vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                      </div>
                    </div>
                    <!-- Detail -->
                    <div
                      class="w-[17.19vw] h-auto text-[0.9375vw] text-[#1E1E1E] font-league leading-[1.40625vw] text-start">
                      “Simple but fun, keeps me coming back every day.”
                    </div>
                  </div>
                </div>
              </div>
              <div class="flex flex-row justify-between">
                <!-- Div 1 -->
                <div class="w-[22vw] relative">
                  <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
                  <!-- FEEDBACK 1 -->
                  <div class="absolute top-[2.08vw] left-[1.146vw] flex flex-col items-start">
                    <!-- name -->
                    <div class="flex flex-row space-x-[0.625vw] items-center">
                      <p class="text-[#1E1E1E] font-emeritus tracking-[-1.1%] text-[1.25vw] leading-[1.35vw]">Sophie
                        K.
                      </p>
                      <div class="flex flex-row space-x-[0.1vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                      </div>
                    </div>
                    <!-- Detail -->
                    <div
                      class="w-[17.19vw] h-auto text-[0.9375vw] text-[#1E1E1E] font-league leading-[1.40625vw] text-start">
                      “Great idle mechanics and smooth controls. Totally recommend!”
                    </div>
                  </div>
                </div>
                <!-- Div 2 -->
                <div class="w-[22vw] relative">
                  <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
                  <!-- FEEDBACK 1 -->
                  <div class="absolute top-[2.08vw] left-[1.146vw] flex flex-col items-start">
                    <!-- name -->
                    <div class="flex flex-row space-x-[0.625vw] items-center">
                      <p class="text-[#1E1E1E] font-emeritus tracking-[-1.1%] text-[1.25vw] leading-[1.35vw]">Olivia
                        B.
                      </p>
                      <div class="flex flex-row space-x-[0.1vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                        <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt=""
                          class="w-[0.9375vw] h-[0.9375vw]">
                      </div>
                    </div>
                    <!-- Detail -->
                    <div
                      class="w-[17.19vw] h-auto text-[0.9375vw] text-[#1E1E1E] font-league leading-[1.40625vw] text-start">
                      “Fun game with nice progression. Enjoy playing while multitasking.”
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- End Section 6 -->

        <!-- Footer -->
        <div class="relative w-full h-auto flex flex-col items-center bg-[#D5D5D5]">
          <div
            class="w-[13.18vw] absolute top-0 right-[13.02vw] flex justify-center items-center text-[#FFF] font-league text-[1.45vw] z-0">
            <img src="../src/assets/img/Desktop/FOOTER/TheTag.webp" alt="" class="w-full">
            <p class="absolute drop-shadow-[0_2px_0.5vw_rgba(0,0,0,0.4)]">Play Free Now!</p>
          </div>
          <img src="../src/assets/img/Desktop/FOOTER/TopBar.webp" alt="" class="w-full h-auto z-10">
          <div class="w-full h-[9.3vw] flex flex-row justify-between">
            <img src="../src/assets/img/Desktop/FOOTER/CotTraiPhai.webp" alt="" class="h-[9.3vw] w-auto">
            <img src="../src/assets/img/Desktop/FOOTER/CotTraiPhai.webp" alt="" class="h-[9.3vw] w-auto scale-x-[-1]">
          </div>

          <!-- Logo -->
          <div
            class="absolute top-[2.5vw] left-[8.8vw] w-[10.8vw] flex flex-col items-center space-y-[-0.1vw] hover:cursor-pointer"
            @click="scrollToRef('home')">
            <p class="text-[#1E1E1E] text-[4.21875vw] uppercase font-emeritus leading-[4.2vw] tracking-[-0.1vw] w-[10.8vw] text-balance
              ">
              IDLE</p>
            <p
              class="text-[#1E1E1E] text-[2.302vw] uppercase font-emeritus leading-[2.3vw] w-[10.8vw] text-balance tracking-[0.1vw]">
              ARENA
            </p>
            <p class="text-[#1E1E1E] text-[0.7vw] font-league leading-[1.25vw] font-thin w-[10.8vw] ">©
              2025 Idle Glory.
              All rights
              reserved.</p>
          </div>

          <!-- Nav select -->
          <div
            class="flex flex-row items-center absolute left-[22.76vw] top-[3.33vw] space-x-[3.177vw] text-[#1E1E1E] text-[1.146vw] font-league font-semibold leading-[1.15vw]">
            <p class="hover:cursor-pointer" @click="scrollToRef('home')">
              Story
            </p>
            <p class="hover:cursor-pointer" @click="scrollToRef('features')">
              Feature
            </p>
            <p class="hover:cursor-pointer" @click="scrollToRef('characters')">
              Gameplay
            </p>
            <p class="hover:cursor-pointer" @click="scrollToRef('community')">
              Community
            </p>
            <p class="hover:cursor-pointer" @click="scrollToRef('contact')">
              Contact
            </p>
            <p class="hover:cursor-pointer">
              FAQs
            </p>
          </div>

          <!-- Join us site -->
          <div
            class="absolute w-[14.74vw] h-[2.6vw] rounded-[0.83vw] bg-[#272725] left-[22.76vw] top-[5.625vw] flex flex-row items-center justify-center space-x-[1.667vw]">
            <p class="text-[1.05vw] font-black font-inter text-[#FFF]">Join us on</p>
            <img src="../src/assets/img/Desktop/FOOTER/FacebookIco.webp" alt="Facebook"
              class="w-[1.25vw] h-[1.25vw] hover:cursor-pointer hover:scale-[1.3] transition-transform duration-300">
            <div class="w-[1.33px] h-[1.4vw] bg-[#565551]"></div>
            <img src="../src/assets/img/Desktop/FOOTER/DiscordIco.webp" alt="Discord"
              class="w-[1.25vw] h-[1.25vw] hover:cursor-pointer hover:scale-[1.3] transition-transform duration-300">
          </div>

          <div class="w-[2px] h-[6.77vw] bg-[#898989] rounded-full absolute right-[32.91vw] top-[2.65625vw]"></div>

          <!-- Download -->
          <div class="flex flex-row space-x-[1.1vw] absolute right-[9.63vw] top-[6.04vw]">
            <!-- Button App Store -->
            <div
              class="w-[9.375vw] h-[2.708vw] rounded-[0.4vw] border-[1px] border-[#A6A6A6] bg-white flex flex-row items-center justify-center space-x-[0.5vw] hover:cursor-pointer">
              <img src="../src/assets/img/Desktop/CTA/CTA_Apple.webp" alt="" class="w-[1.44vw] h-[1.73vw]">
              <img src="../src/assets/img/Desktop/CTA/AppStore.png" alt="" class="w-[5.52vw]">
            </div>
            <!-- Button Google Play -->
            <div
              class="w-[9.375vw] h-[2.708vw] rounded-[0.4vw] border-[1px] border-[#A6A6A6] bg-white flex flex-row items-center justify-center space-x-[0.5vw] hover:cursor-pointer">
              <img src="../src/assets/img/Desktop/CTA/CTA_GG_Play.webp" alt="" class="w-[1.6vw] h-[1.74vw]">
              <img src="../src/assets/img/Desktop/CTA/GGPLay.png" alt="" class="w-[5.8875vw]">
            </div>
          </div>
        </div>
        <!-- End Footer -->

      </div>
    </div>
    <!-- Mobile -->
    <div v-if="isMobile" class="w=full h-auto">
      <div class="relative w-full h-[865vw] flex flex-col bg-[#D5D5D5] items-center">
        <!-- Đoạn này để back vàng -->
        <img src="../src/assets/img/Mobile/Homepage/lightvang.webp" alt="" class="absolute top-0 left-0 w-full h-auto">
        <img src="../src/assets/img/Mobile/Homepage/ImgLeftHome.webp" alt=""
          class="w-[68.7vw] absolute top-[25.4vw] left-0">
        <img src="../src/assets/img/Mobile/Homepage/ImgRightHome.webp" alt=""
          class="w-[81.5vw] absolute top-[51.3vw] right-[0vw]">

        <!-- Text -->
        <div class="absolute top-[150vw] space-y-[2vw] w-full flex flex-col items-center">
          <p class="text-center text-[#1E1E1E] text-[8.14vw] font-emeritus leading-[8.15vw] tracking-[-1.1%]">An
            Exciting World<br />
            of Adventure</p>
          <p class="text-[#1E1E1E] text-center text-[3.05vw] font-lexend">Summon your champions to the battlefield of
            Idle Area! Call forth mighty warriors, upgrade their power, and forge an unstoppable team. The fight for
            glory begins—answer the call now!</p>
          <div class="flex items-center justify-center w-[35.6vw] relative">
            <img src="../src/assets/img/Desktop/HomePage/button.webp" alt="" class="w-full h-auto">
            <p class="font-lexend text-[#1E1E1E] text-[3.05vw] text-center absolute uppercase font-bold leading-[3vw]">
              Join now</p>
          </div>
        </div>

        <!-- Conquer Chapters -->
        <div class="absolute top-[193vw] w-full h-[133.6vw] flex justify-center">
          <img src="../src/assets/img/Desktop/HomePage/ball.webp" alt=""
            class="w-[16vw] absolute top-[18.17vw] left-[19.6vw]">
          <img src="../src/assets/img/Desktop/HomePage/light-purple.webp" alt=""
            class="absolute w-full h-auto bottom-[20vw]">
          <img src="../src/assets/img/Desktop/HomePage/cybog.webp" alt="" class="w-[61.83vw] absolute top-[11.96vw]">
          <img src="../src/assets/img/Desktop/HomePage/ball-1.webp" alt=""
            class="w-[9vw] absolute top-[39vw] left-[3.8vw]">
          <img src="../src/assets/img/Desktop/HomePage/ball-2.webp" alt=""
            class="w-[20.3vw] absolute top-[35.36vw] right-[5vw]">
          <!-- Text -->
          <div class="w-full flex flex-col items-center absolute top-[55vw] space-y-[2vw]">
            <p class="text-[#1E1E1E] text-[8.14vw] font-emeritus leading-[8vw] tracking-[-1.1%] text-center">Conquer
              Chapters<br />
              Climb the Stages</p>
            <p class="text-[#1e1e1e] text-[3.05vw] font-lexend text-center leading-[4.5vw]">
              Lead your heroes through an epic journey,<br />
              battling enemies and bosses across countless<br />
              chapters and
              stages.
            </p>
          </div>

          <!-- purple smoke -->
          <img src="../src/assets/img/Mobile/Conquer/ConquerPurpleSmoke.webp" alt=""
            class="w-full h-auto absolute bottom-0">

          <img src="../src/assets/img/Mobile/Adventure/boardgame.webp" alt=""
            class="w-full h-auto absolute bottom-[-15vw]">
        </div>

        <div
          class="absolute top-[325vw] w-full h-[219.6vw] rounded-[3.56vw] bg-gradient-to-b from-[#E8E8E8] to-transparent"
          style="box-shadow: 0 0 80px 0 #00000060;">
          <div class="absolute flex flex-col items-center w-full bottom-[3.05vw] space-y-[3.8vw]">
            <img src="../src/assets/img/Desktop/Experience/game.webp" alt="" class="w-[95vw] h-auto">
            <img src="../src/assets/img/Desktop/Experience/reward.webp" alt="" class="w-[95vw] h-auto">
          </div>
          <div class="absolute w-[95vw] flex flex-col items-start left-[2.5vw] top-[4.07vw]">
            <p class="text-[#1E1E1E] text-[7.8vw] tracking-[-1.1%] font-emeritus leading-[8vw]">Experience an exciting
            </p>
            <p class="mt-[3vw] text-[#F9791C] uppercase font-emeritus text-[19.3vw] tracking-[-0.3vw] leading-[19vw]">
              Idle RPG</p>
            <p class="text-[#1E1E1E] text-[3.05vw] font-lexend text-start leading-[4.5vw] mt-[7vw]">
              Immerse yourself in a thrilling idle RPG - battles never stop.
              <br /> Earn valuable rewards even while you’re offline
            </p>
          </div>
        </div>

        <!-- Adventure -->
        <div class="absolute top-[545vw] w-full h-[314.122vw] flex flex-col justify-center">
          <img src="../src/assets/img/Mobile/Adventure/AdventureActor.webp" alt="" class="w-full absolute top-0">
          <div class="absolute top-[80vw] w-full flex flex-col items-center">
            <p class="text-[#F9791C] text-[13.99vw] w-[95vw] font-emeritus uppercase leading-[14vw] mr-[2.5vw]">
              Adventure</p>
            <p class="text-[#1E1E1E] text-[8.14vw] font-emeritus leading-[8vw] mt-[3vw]">Conquer all challenges</p>
            <p
              class="text-[#1E1E1E] text-[3.05vw] font-lexend leading-[3vw] mt-[5vw] tracking-[-0.1vw] w-[95vw] text-end">
              Immerse
              yourself in a thrilling
              idle RPG -
              battles never stop.</p>
          </div>
          <div class="absolute bottom-[0vw] w-full flex flex-col space-y-[3.8vw] items-center">
            <img src="../src/assets/img/Desktop/Adventure/adventure1.webp" alt="" class="w-[95vw] h-auto">
            <img src="../src/assets/img/Desktop/Adventure/adventure2.webp" alt="" class="w-[95vw] h-auto">
            <img src="../src/assets/img/Desktop/Adventure/adventure3.webp" alt="" class="w-[95vw] h-auto">
            <img src="../src/assets/img/Desktop/Adventure/adventure4.webp" alt="" class="w-[95vw] h-auto">
            <img src="../src/assets/img/Desktop/Adventure/adventure5.webp" alt="" class="w-[95vw] h-auto">
          </div>
        </div>
      </div>

      <!-- Thẻ để chuyển - để lại làm 1 lượt -->
      <div class="relative w-full h-[244vw] bg-white overflow-hidden">
        <!-- BACKGROUND LAYER -->
        <div class="absolute inset-0 z-0">
          <img v-for="(s, i) in slides" :key="'mbg-' + s.key" :src="mBackgroundMap[s.key].src"
            class="w-full h-auto absolute left-0 top-0 background-img-mobile m-layer" :class="mStateClass(i)"
            draggable="false" />
        </div>

        <!-- MODEL LAYER -->
        <div class="absolute inset-0 z-10">
          <img v-for="(s, i) in slides" :key="'mmodel-' + s.key" :src="mModelMap[s.key].src"
            class="absolute m-layer model-img-mobile" :style="mModelStyleFor(i)" :class="mStateClass(i)"
            draggable="false" />
        </div>

        <!-- SKILL LAYER -->
        <div class="absolute inset-x-0 bottom-[9.16vw] z-20">
          <img v-for="(s, i) in slides" :key="'mskill-' + s.key" :src="mSkillMap[s.key].src"
            class="w-full h-auto absolute left-0 bottom-0 m-layer skill" :class="mStateClass(i)" draggable="false" />
        </div>

        <!-- BUTTONS -->
        <div class="absolute top-[148vw] right-[6.615vw] flex flex-row w-[53.43vw] justify-between z-30 px-[2vw]">
          <img src="../src/assets/img/Desktop/CHARACTER_WEBP/buttonleft.webp" class="w-[7.6vw] h-auto transition"
            :class="mCanPrev ? 'hover:cursor-pointer' : 'grayscale opacity-50 pointer-events-none'" @click="mPrev"
            :aria-disabled="!mCanPrev" />
          <img src="../src/assets/img/Desktop/CHARACTER_WEBP/buttonright.webp" class="w-[7.6vw] h-auto transition"
            :class="mCanNext ? 'hover:cursor-pointer' : 'grayscale opacity-50 pointer-events-none'" @click="mNext"
            :aria-disabled="!mCanNext" />
        </div>

        <!-- BUTTON BOOKING -->
        <div class="absolute top-[175.06vw] w-full h-auto flex items-center justify-center">
          <img src="../src/assets/img/Desktop/CHARACTER_WEBP/level.webp" alt="" class="w-[55.2vw] h-auto">
        </div>
      </div>

      <!-- 5 actors -->
      <div class="relative w-full h-[440vw] bg-[#FFFAEB]">
        <img src="../src/assets/img/Mobile/ACTOR/BackTop.webp" alt="" class="w-full h-auto absolute top-0">
        <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Xinzhao.webp" alt=""
          class="w-[50.6vw] absolute top-[11.96vw] right-[3.3vw]">

        <!-- Text -->
        <div class="absolute top-[62vw] w-full flex flex-col items-center space-y-[5vw]">
          <!-- 1 -->
          <div class="w-[95vw] flex flex-col">
            <div class="flex flex-row w-full items-center justify-start space-x-[3vw]">
              <p class="text-[#1e1e1e] text-[5.089vw] font-emeritus leading-[5vw]">Awaken Ember</p>
              <img src="../src/assets/img/Mobile/ACTOR/AwakenEmber.webp" alt="" class="w-[8.4vw]">
            </div>
            <p class="text-[#1e1e1e] text-[3.05vw] font-league">Description: This group of characters carries within
              them a mysterious, primal energy, awakened from a forgotten world. The characters in Awaken Ember
              possess ancient powers and the ability to control fire or natural elements. They are not only powerful
              but also exude an aura of mysticism, inspired by ancient creatures and arcane magic.<br />
              Key Features:<br />
              • Supernatural powers derived from fire or natural elements.<br />
              • Ability to heal quickly thanks to mystical energy.<br />
              • Can summon creatures or natural elements to
              assist in combat.</p>
          </div>
          <!-- 2 -->
          <div class="w-[95vw] flex flex-col">
            <div class="flex flex-row w-full items-center justify-start space-x-[3vw]">
              <p class="text-[#1e1e1e] text-[5.089vw] font-emeritus leading-[5vw]">Beast</p>
              <img src="../src/assets/img/Mobile/ACTOR/Beast.webp" alt="" class="w-[8.4vw]">
            </div>
            <p class="text-[#1e1e1e] text-[3.05vw] font-league">Description: The warriors in the Beast group possess
              extraordinary strength, derived from their wild instincts and powerful physiques. They are inspired by
              fierce beasts, embodying unmatched strength and primal combat prowess. Their battle style is aggressive
              and relentless, never hesitating to charge into battle with full force.<br />
              Key Features:<br />
              • Exceptional physical strength and speed.<br />
              • Powerful close-range combat abilities with devastating attacks.<br />
              • Special expertise in using heavy weapons or combat techniques tied to nature.</p>
          </div>
          <!-- 3 -->
          <div class="w-[95vw] flex flex-col">
            <div class="flex flex-row w-full items-center justify-start space-x-[3vw]">
              <p class="text-[#1e1e1e] text-[5.089vw] font-emeritus leading-[5vw]">Cyborg</p>
              <img src="../src/assets/img/Mobile/ACTOR/Cyborg.webp" alt="" class="w-[8.4vw]">
            </div>
            <p class="text-[#1e1e1e] text-[3.05vw] font-league">Description: The Cyborg group is a fusion of man and
              machine, where warriors are enhanced with advanced technology. These characters have mechanical body parts
              that significantly boost their physical strength and combat abilities. They also possess the ability to
              control machinery and harness cutting-edge technology in battle.<br />
              Key Features:<br />
              • A combination of human body and robotic parts, enhancing strength and speed.<br />
              • Capable of using advanced technology and controlling devices remotely.<br />
              • Highly durable in long battles, with quick self-repair abilities thanks to technology.</p>
          </div>
          <!-- 4 -->
          <div class="w-[95vw] flex flex-col">
            <div class="flex flex-row w-full items-center justify-start space-x-[3vw]">
              <p class="text-[#1e1e1e] text-[5.089vw] font-emeritus leading-[5vw]">Human</p>
              <img src="../src/assets/img/Mobile/ACTOR/Human.webp" alt="" class="w-[7.3vw]">
            </div>
            <p class="text-[#1e1e1e] text-[3.05vw] font-league">Description: This group consists of human warriors who
              possess special abilities without relying on technology or magic. These characters are flexible and
              skilled, ranging from experienced fighters to expert explorers. They excel in combat through strategy,
              dexterity, and adaptability in tough situations.<br />
              Key Features:<br />
              • Diverse combat skills and tactics.<br />
              • High flexibility, able to use a wide range of weapons and gear.<br />
              • Resilience and the ability to adapt to any battlefield.</p>
          </div>
          <!-- 5 -->
          <div class="w-[95vw] flex flex-col">
            <div class="flex flex-row w-full items-center justify-start space-x-[3vw]">
              <p class="text-[#1e1e1e] text-[5.089vw] font-emeritus leading-[5vw]">Ultron</p>
              <img src="../src/assets/img/Mobile/ACTOR/Ultron.webp" alt="" class="w-[7.3vw]">
            </div>
            <p class="text-[#1e1e1e] text-[3.05vw] font-league">Description: The Ultron group features characters with
              superior technological abilities, blending artificial intelligence with enhanced strength. They have
              intelligent minds and systems capable of analyzing and predicting battles instantly. The characters in the
              Ultron group can create powerful weapons and maintain constant offensive capabilities.<br />
              Key Features:<br />
              • Possess artificial intelligence and the ability to optimize combat strategies.<br />
              • Can control high-tech weapons and create support tools for combat.<br />
              • Consistent strength and the ability to battle with superior capabilities, always staying one step ahead
              of the enemy.</p>
          </div>
        </div>

        <!-- Image bottom -->
        <img src="../src/assets/img/Mobile/ACTOR/BackBot.webp" alt="" class="w-full h-auto absolute bottom-0">

        <img src="../src/assets/img/Desktop/ACTOR/ACTOR_Kathus.webp" alt=""
          class="w-[47.5vw] absolute bottom-[5.1vw] left-[3.1vw]">
      </div>

      <!-- CTA -->
      <div class="relative w-full h-[505.8vw] flex flex-col items-center bg-[#FFFAEB]">
        <img src="../src/assets/img/Desktop/CTA/CTA_Wheel_back.webp" alt="" class="w-[87.8vw] absolute top-[25.4vw]">
        <img src="../src/assets/img/Desktop/CTA/CTA_Darius.webp" alt="" class="w-[83vw] absolute top-[29.5vw]">
        <!-- Text -->
        <div class="absolute top-[90.33vw] w-full h-auto flex flex-col items-center">
          <p class="w-[97vw] text-center text-[#1e1e1e] text-[7.3vw] font-emeritus leading-[7.884vw] tracking-[-1.1%]">
            Kickstart Your
            <br />
            Adventure in Style
          </p>
          <p class="w-[87vw] text-center text-[#1e1e1e] text-[3.56vw] font-league leading-[4.5vw]">
            Log in for the first time to claim valuable gifts and limited-<br />
            time bonuses! Boost your journey, unlock exclusive gear, and<br />
            start your gaming adventure with excitement.
          </p>
          <div class="w-[35.6vw] mt-[6.1vw] justify-center items-center relative flex">
            <img src="../src/assets/img/Desktop/HomePage/button.webp" alt="" class="w-full">
            <p class="absolute text-[#1e1e1e] text-[3.7vw] font-league uppercase font-bold leading-[4.2vw]">Free to play
            </p>
          </div>
        </div>

        <!-- line -->
        <div class="absolute top-[148vw] w-full flex flex-col items-center">
          <div class="w-full h-[15.27vw] flex flex-col justify-center items-center">
            <img src="../src/assets/img/Mobile/CTA/bg-playnow.webp" alt="" class="w-full h-auto">
            <p class="absolute text-[#1e1e1e] text-[5.08vw] font-emeritus"> Play Now – Anywhere!</p>
          </div>
          <!-- button download -->
          <div class="w-full h-auto mt-[3.82vw] flex flex-row justify-center items-center space-x-[3.7vw]">
            <div
              class="w-[45.8vw] h-[13.28vw] rounded-[2vw] bg-white border-[1px] border-[#A6A6A6] flex flex-row items-center justify-center space-x-[1.5vw]">
              <img src="../src/assets/img/Desktop/CTA/CTA_Apple.webp" alt="" class="w-[7.3vw]">
              <img src="../src/assets/img/Desktop/CTA/AppStore.png" alt="" class="w-[27.06vw]">
            </div>
            <div
              class="w-[45.8vw] h-[13.28vw] rounded-[2vw] bg-white border-[1px] border-[#A6A6A6] flex flex-row items-center justify-center space-x-[1.5vw]">
              <img src="../src/assets/img/Desktop/CTA/CTA_GG_Play.webp" alt="" class="w-[7.3vw]">
              <img src="../src/assets/img/Desktop/CTA/GGPLay.png" alt="" class="w-[27.06vw]">
            </div>
          </div>

          <!-- discord/ facebook -->
          <div class="w-full h-[33vw] flex flex-col justify-center mt-[3.9vw] overflow-hidden">
            <div class="w-full h-[20.3vw] relative flex flex-col items-center">
              <div class="w-full h-[12.72vw] bg-gradient-to-tr from-[#BA81FF] to-[#FFC3F9] absolute bottom-0"></div>
              <img src="../src/assets/img/Desktop/CTA/CTA_Discord_CaSau.webp" alt=""
                class="w-[30.3vw] absolute bottom-0 left-[2.5vw]">
              <img src="../src/assets/img/Desktop/CTA/CTA_Discord.webp" alt=""
                class="w-[43vw] absolute bottom-[-3.5vw]">
            </div>
            <div
              class="w-full h-[12.72vw] bg-gradient-to-br from-[#E1F1FF] to-[#78B8FF] relative flex items-center justify-center">
              <img src="../src/assets/img/Desktop/CTA/CTA_Facebook.webp" alt="" class="absolute w-[33.8vw]">
            </div>
            <img src="../src/assets/img/Desktop/CTA/CTA_Facebook_Blitzcrank.webp" alt=""
              class="w-[21.3vw] absolute bottom-[-2vw] right-[4.3vw]">
          </div>
          <!-- Feedback -->
          <div class="relative w-full h-auto flex flex-col items-center">
            <img src="../src/assets/img/Desktop/CTA/CTA_O_tren.webp" alt="" class="w-full absolute top-0">
          </div>
        </div>

        <!-- Feedback -->
        <div class="absolute top-[227.5vw] w-full flex flex-col space-y-[4.63vw] items-center">
          <div class="w-[95vw] relative">
            <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
            <div class="flex flex-col items-start absolute top-[9.93vw] left-[5.2vw]">
              <div class="flex flex-row space-x-[2.5vw]">
                <p class="text-[#1e1e1e] text-[5.55vw] font-emeritus leading-[5.55vw]">Jake M</p>
                <div class="flex flex-row space-x-[1.5px]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                </div>
              </div>
              <p class="mt-[2vw] text-[#1e1e1e] font-league text-[4.17vw] leading-[6vw]">“Idle Arena is super chill and
                addictive.<br /> Perfect for quick breaks!”</p>
            </div>
          </div>
          <!-- 2 -->
          <div class="w-[95vw] relative">
            <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
            <div class="flex flex-col items-start absolute top-[9.93vw] left-[5.2vw]">
              <div class="flex flex-row space-x-[2.5vw]">
                <p class="text-[#1e1e1e] text-[5.55vw] font-emeritus leading-[5.55vw]">Emily R</p>
                <div class="flex flex-row space-x-[1.5px]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                </div>
              </div>
              <p class="mt-[2vw] text-[#1e1e1e] font-league text-[4.17vw] leading-[6vw]">“Love the graphics and easy
                gameplay.<br />Great way to kill time.”</p>
            </div>
          </div>
          <!-- 3 -->
          <div class="w-[95vw] relative">
            <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
            <div class="flex flex-col items-start absolute top-[9.93vw] left-[5.2vw]">
              <div class="flex flex-row space-x-[2.5vw]">
                <p class="text-[#1e1e1e] text-[5.55vw] font-emeritus leading-[5.55vw]">Noah T</p>
                <div class="flex flex-row space-x-[1.5px]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                </div>
              </div>
              <p class="mt-[2vw] text-[#1e1e1e] font-league text-[4.17vw] leading-[6vw]">“Perfect for casual gaming.
                Easy to pick up,<br /> hard to put down.”</p>
            </div>
          </div>
          <!-- 4 -->
          <div class="w-[95vw] relative">
            <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
            <div class="flex flex-col items-start absolute top-[9.93vw] left-[5.2vw]">
              <div class="flex flex-row space-x-[2.5vw]">
                <p class="text-[#1e1e1e] text-[5.55vw] font-emeritus leading-[5.55vw]">Liam S</p>
                <div class="flex flex-row space-x-[1.5px]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                </div>
              </div>
              <p class="mt-[2vw] text-[#1e1e1e] font-league text-[4.17vw] leading-[6vw]">“Simple but fun, keeps me
                coming back<br />every day.”</p>
            </div>
          </div>
          <!-- 5 -->
          <div class="w-[95vw] relative">
            <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
            <div class="flex flex-col items-start absolute top-[9.93vw] left-[5.2vw]">
              <div class="flex flex-row space-x-[2.5vw]">
                <p class="text-[#1e1e1e] text-[5.55vw] font-emeritus leading-[5.55vw]">Sophie K.</p>
                <div class="flex flex-row space-x-[1.5px]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                </div>
              </div>
              <p class="mt-[2vw] text-[#1e1e1e] font-league text-[4.17vw] leading-[6vw]">“Great idle mechanics and
                smooth controls.<br /> Totally recommend!”</p>
            </div>
          </div>
          <!-- 6 -->
          <div class="w-[95vw] relative">
            <img src="../src/assets/img/Desktop/CTA/CTA_Feedback.webp" alt="" class="w-full h-auto">
            <div class="flex flex-col items-start absolute top-[9.93vw] left-[5.2vw]">
              <div class="flex flex-row space-x-[2.5vw]">
                <p class="text-[#1e1e1e] text-[5.55vw] font-emeritus leading-[5.55vw]">Olivia B.</p>
                <div class="flex flex-row space-x-[1.5px]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                  <img src="../src/assets/img/Desktop/CTA/CTA_feedback_star.webp" alt="" class="w-[4.17vw] h-[4.17vw]">
                </div>
              </div>
              <p class="mt-[2vw] text-[#1e1e1e] font-league text-[4.17vw] leading-[6vw]">“Fun game with nice
                progression. Enjoy<br /> playing while multitasking.”</p>
            </div>
          </div>
        </div>

        <!-- The bottom -->
        <div class="absolute bottom-0 w-full h-auto flex flex-col items-center">
          <img src="../src/assets/img/Desktop/CTA/CTA_Man_Last.webp" alt=""
            class="w-[59.5vw] absolute bottom-[2.5vw] left-[14.76vw]">
          <img src="../src/assets/img/Desktop/CTA/CTA_O_duoi.webp" alt="" class="w-full h-auto absolute bottom-0">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import lib
import { ref, onMounted, computed, onBeforeUnmount, watch } from "vue";
import Lenis from "@studio-freight/lenis";

// export
export default {
  name: 'App',
  setup() {
    const homeFrame = ref(null);
    const gamePlay = ref(null);
    let lenis;
    let rafId = 0;
    const windowWidth = ref(window.innerWidth);
    const isMobile = computed(() => windowWidth.value <= 768);
    const initialIsMobile = ref(isMobile.value);

    const selectedIndex = ref(0);
    const adventure1 = new URL('../src/assets/img/Desktop/Adventure/adventure1.webp', import.meta.url).href;
    const adventure2 = new URL('../src/assets/img/Desktop/Adventure/adventure2.webp', import.meta.url).href;
    const adventure3 = new URL('../src/assets/img/Desktop/Adventure/adventure3.webp', import.meta.url).href;
    const adventure4 = new URL('../src/assets/img/Desktop/Adventure/adventure4.webp', import.meta.url).href;
    const adventure5 = new URL('../src/assets/img/Desktop/Adventure/adventure5.webp', import.meta.url).href;
    // Declare variables
    const secHome = ref(null);
    const secFeatures = ref(null);
    const secCharacters = ref(null);
    const secCampaign = ref(null);
    const secCommunity = ref(null);
    const secContact = ref(null);

    const STAGE_W = '26vw';
    const STAGE_H = '49.167vw';

    const glowColors = ['#FF91B2', '#5AC5FF', '#FCE671', '#FF0000', '#00FF9A'];
    const glowColor = computed(() => glowColors[current.value]);

    const handleResize = () => {
      windowWidth.value = window.innerWidth;
      if (isMobile.value !== initialIsMobile.value) {
        // window.location.reload(true);
        initialIsMobile.value = isMobile.value;
      }
    };

    const startRaf = () => {
      const loop = (time) => {
        // dùng window.__lenis để tránh closure giữ lenis cũ
        const l = window.__lenis;
        if (l) l.raf(time);
        rafId = requestAnimationFrame(loop);
      };
      rafId = requestAnimationFrame(loop);
    };

    const stopRaf = () => {
      if (rafId) cancelAnimationFrame(rafId);
      rafId = 0;
    };

    const initLenis = () => {
      if (lenis) return;
      lenis = new Lenis({
        lerp: 0.09,
        wheelMultiplier: 1.6,
        touchMultiplier: 1.0,
        smoothWheel: true,
        smoothTouch: true
      });
      window.__lenis = lenis;
      startRaf();
    };

    const destroyLenis = () => {
      if (lenis) {
        lenis.destroy();
        lenis = null;
      }
      window.__lenis = null;
      stopRaf();
    };

    const actorMap = {
      yumi: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/yumimodel.webp', import.meta.url).href,
        width: '40.8vw', right: '12vw', bottom: '-7.5vw',
        offsetY: '0vw',
        enterFrom: '0vw',
      },
      zat: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/zatmodel.webp', import.meta.url).href,
        width: '35.4vw', right: '4.43vw', bottom: '-10vw',
        offsetY: '0vw',
        enterFrom: '0vw',
      },
      kong: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/kongyolumodel.webp', import.meta.url).href,
        width: '41.145vw', right: '1.51vw', bottom: '-7vw', offsetY: '0vw',
        enterFrom: '0vw',
      },
      ivy: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/lucianmodel.webp', import.meta.url).href,
        width: '36.146vw', right: '2.96875vw', bottom: '-8vw', offsetY: '0vw',
        enterFrom: '0vw',
      },
      drax: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/krysysmodel.webp', import.meta.url).href,
        width: '18.073vw', right: '18.646vw', bottom: '-5vw', offsetY: '0vw',
        enterFrom: '0vw',
      },
    };

    const current = ref(0);

    const slides = [
      { key: "yumi", subtitle: "The Crazed Cleaver" },
      { key: "zat", subtitle: "Wicked Bombardier" },
      { key: "kong", subtitle: "Millenium Beast" },
      { key: "ivy", subtitle: "The Hope Guardian" },
      { key: "drax", subtitle: "The Unyielding Flame" },
    ];

    const backGradients = [
      'linear-gradient(135deg, #FF99B8 0%, #F6CCD9 100%)', // YUMI
      'linear-gradient(135deg, #9AD7FF 0%, #D0EEFF 100%)', // ZAT
      'linear-gradient(135deg, #FFDE7A 0%, #FFF2B2 100%)', // KONG
      'linear-gradient(135deg, #FF7F7F 0%, #D13737 100%)', // 4
      'linear-gradient(135deg, #00FF98 0%, #86FFE4 100%)', // 5
    ];

    const line1Colors = ['#FF71AC', '#4EC3FF', '#FFB200', '#FF0000', '#007E52']

    const actorImages = [
      new URL('../src/assets/img/Desktop/CHARACTER_WEBP/yumimodel.webp', import.meta.url).href,
      new URL('../src/assets/img/Desktop/CHARACTER_WEBP/zatmodel.webp', import.meta.url).href,
      new URL('../src/assets/img/Desktop/CHARACTER_WEBP/kongyolumodel.webp', import.meta.url).href,
      new URL('../src/assets/img/Desktop/CHARACTER_WEBP/lucianmodel.webp', import.meta.url).href,
      new URL('../src/assets/img/Desktop/CHARACTER_WEBP/krysysmodel.webp', import.meta.url).href,
    ];

    const backCoverMap = {
      yumi: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/YumiCover.webp', import.meta.url).href,
        top: '0', right: '0', height: STAGE_H,
        offsetX: '0', offsetY: '0', scale: 1, rotate: '0deg',
      },
      zat: { src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/ZatCover.webp', import.meta.url).href, top: '0', right: '0', height: STAGE_H },
      kong: { src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/KongYoluCover.webp', import.meta.url).href, top: '0', right: '0', height: STAGE_H },
      ivy: { src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/LucianCover.webp', import.meta.url).href, top: '0', right: '0', height: STAGE_H },
      drax: { src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/KrysusCover.webp', import.meta.url).href, top: '0', right: '0', height: STAGE_H },
    };

    const actorOffsets = ['0vw', '-1vw', '1vw', '0.5vw', '-0.75vw'];

    // Tính toán binding
    const backGradient = computed(() => backGradients[current.value])
    const line1Color = computed(() => line1Colors[current.value])
    const actorOffset = computed(() => actorOffsets[current.value])

    const backCoverWrapStyleFor = (i) => {
      const c = backCoverMap[slides[i].key] || {};
      return {
        position: 'absolute',
        top: c.top ?? '0',
        right: c.right ?? '0',
        left: 'auto',
        bottom: 'auto',
        height: c.height ?? STAGE_H,
        width: 'auto',
      };
    };

    const backCoverImgStyleFor = (i) => {
      const c = backCoverMap[slides[i].key] || {};
      const tx = c.imgTranslateX ?? c.offsetX ?? '0';
      const ty = c.imgTranslateY ?? c.offsetY ?? '0';
      const sc = c.imgScale ?? c.scale ?? 1;
      const rot = c.imgRotate ?? c.rotate ?? '0deg';
      return {
        transform: `translate(${tx}, ${ty}) scale(${sc}) rotate(${rot})`,
        height: '100%',
        width: 'auto',
      };
    };

    // Text back offset
    const textOffset = computed(() => `-${current.value * 60}vw`)

    function next() {
      if (!canNext.value) return;
      goTo(current.value + 1);
    }
    function prev() {
      if (!canPrev.value) return;
      goTo(current.value - 1);
    }

    const actorWrapStyleFor = (i) => {
      const c = actorMap[slides[i].key] || {};
      const style = {
        width: c.width || '40vw',
        height: '49.167vw',
      };

      if (c.left != null) { style.left = c.left; style.right = 'auto'; }
      else { style.right = c.right ?? '10vw'; style.left = 'auto'; }

      if (c.top != null) { style.top = c.top; style.bottom = 'auto'; }
      else { style.bottom = c.bottom ?? '0vw'; style.top = 'auto'; }

      if (c.slotTransform) style.transform = c.slotTransform;
      return style;
    };

    const actorImgStyleFor = (i) => {
      const c = actorMap[slides[i].key] || {};
      const tx = c.imgTranslateX ?? c.offsetX ?? '0';
      const ty = c.imgTranslateY ?? c.offsetY ?? '0';
      const sc = c.imgScale ?? c.scale ?? 1;
      const rot = c.imgRotate ?? c.rotate ?? '0deg';
      return {
        transform: `translate(${tx}, ${ty}) scale(${sc}) rotate(${rot})`,
        width: '100%'
      };
    };

    const actorSlotClass = (i) => {
      if (isAnimating.value) {
        if (i === prevIndex.value) {
          return direction.value === 'up' ? 'anim-up-out' : 'anim-down-out';
        }
        if (i === current.value) {
          return direction.value === 'up' ? 'anim-up-in' : 'anim-down-in';
        }
        return 'hidden-slot';
      }
      return i === current.value ? 'shown-slot' : 'hidden-slot';
    };

    const selectThumb = (i) => {
      if (selectedIndex.value !== i) selectedIndex.value = i
    };

    const basisStyle = (i) => ({
      '--basis': selectedIndex.value === i ? '32.6vw' : '12.08vw',
      zIndex: selectedIndex.value === i ? 10 : 1,
    });

    const imgStyle = (i) => ({
      filter: selectedIndex.value === i ? 'grayscale(0%)' : 'grayscale(100%)',
    });

    const growStyle = (i) => ({
      '--g': selectedIndex.value === i ? 2.6 : 1,
      zIndex: selectedIndex.value === i ? 10 : 1,
    });

    const ringClass = (i) => selectedIndex.value === i ? 'ring-on' : 'ring-off';

    const NAV_OFFSET_VW = 6.25;

    const getOffsetPx = () => (NAV_OFFSET_VW / 100) * window.innerWidth;

    const scrollToRef = (key) => {
      const map = {
        home: secHome,
        features: secFeatures,
        characters: secCharacters,
        campaign: secCampaign,
        community: secCommunity,
        contact: secContact,
      };
      const target = map[key]?.value;
      if (!target) return;

      const offset = -getOffsetPx();

      if (window.__lenis) {
        window.__lenis.scrollTo(target, { offset });
      } else {
        const y = target.getBoundingClientRect().top + window.scrollY + offset;
        window.scrollTo({ top: y, behavior: "smooth" });
      }
    };

    const cardMap = {
      yumi: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/yumicard.webp', import.meta.url).href,
        width: '20.15625vw', left: '5.2vw', bottom: '4.375vw', rotate: '0deg',
      },
      zat: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/zatcard.webp', import.meta.url).href,
        width: '20.15625vw', left: '5.2vw', bottom: '4.375vw', rotate: '0deg',
      },
      kong: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/kongyolu.webp', import.meta.url).href,
        width: '20.15625vw', left: '5.2vw', bottom: '4.375vw', rotate: '0deg',
      },
      ivy: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/lucian.webp', import.meta.url).href,
        width: '20.15625vw', left: '5.2vw', bottom: '4.375vw', rotate: '0deg',
      },
      drax: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/krysus.webp', import.meta.url).href,
        width: '20.15625vw', left: '5.2vw', bottom: '4.375vw', rotate: '0deg',
      },
    };

    const revealMaskStyle = {
      WebkitMaskImage: 'linear-gradient(to right, rgba(0,0,0,0) 0%, rgba(0,0,0,1) 30%)',
      maskImage: 'linear-gradient(to right, rgba(0,0,0,0) 0%, rgba(0,0,0,1) 30%)',
      WebkitMaskRepeat: 'no-repeat',
      maskRepeat: 'no-repeat',
      WebkitMaskSize: '100% 100%',
      maskSize: '100% 100%',
    };

    const actorWrapStyle = computed(() => {
      const c = actorMap[currentKey.value] || {};
      return {
        width: c.width || '40vw',
        right: c.right || '10vw',
        bottom: c.bottom || '0vw',
      };
    });

    const actorImgStyle = computed(() => {
      const c = actorMap[currentKey.value] || {};
      const t = [
        c.offsetX && `translateX(${c.offsetX})`,
        c.offsetY && `translateY(${c.offsetY})`,
        c.scale && `scale(${c.scale})`,
        c.rotate && `rotate(${c.rotate})`,
      ].filter(Boolean).join(' ') || 'none';
      return { transform: t, width: '100%' };
    });

    const cardSrc = computed(() => cardMap[currentKey.value]?.src || '');
    const cardStyle = computed(() => {
      const c = cardMap[currentKey.value] || {};
      return {
        width: c.width ?? '20.15625vw',
        left: c.left ?? '5.2vw',
        bottom: c.bottom ?? '4.375vw',
        transform: `translateZ(0) rotate(${c.rotate ?? '0deg'})`,
      };
    });

    const wheelDeg = ref(0);
    const wheelStyle = computed(() => ({
      transform: `rotate(${wheelDeg.value}deg)`
    }));

    // Block turn right - left
    const canPrev = computed(() => current.value > 0);
    const canNext = computed(() => current.value < slides.length - 1);

    const prevIndex = ref(0);
    const direction = ref('up');
    const isAnimating = ref(false);
    const ANIM_MS = 1200;

    const goTo = (i) => {
      if (i < 0 || i > slides.length - 1) return;
      if (i === current.value) return;
      if (isAnimating.value) return;

      prevIndex.value = current.value;
      direction.value = i > current.value ? 'down' : 'up';
      current.value = i;
      isAnimating.value = true;

      wheelDeg.value = (wheelDeg.value + (prevIndex.value - i) * 20) % 360;

      setTimeout(() => { isAnimating.value = false; }, ANIM_MS);
    };

    // --- MOBILE SLIDER STATE ---
    const mCurrent = ref(0);
    const mCanPrev = computed(() => mCurrent.value > 0);
    const mCanNext = computed(() => mCurrent.value < slides.length - 1);
    const mPrev = () => { if (mCanPrev.value) mCurrent.value--; };
    const mNext = () => { if (mCanNext.value) mCurrent.value++; };

    const mStateClass = (i) => (i === mCurrent.value ? 'm-show' : 'm-hide');

    // Backgrounds (đổi src theo tên file bạn có; tránh khoảng trắng trong file name)
    const mBackgroundMap = {
      yumi: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/backyumi .webp', import.meta.url).href },
      zat: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/backzat.webp', import.meta.url).href },
      kong: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/backkongyolu.webp', import.meta.url).href },
      ivy: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/backlucian.webp', import.meta.url).href },
      drax: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/backkrysus.webp', import.meta.url).href },
    };

    // Models (giữ “đặc tính riêng” từng model: width/top/left)
    const mModelMap = {
      yumi: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/yumimodel.webp', import.meta.url).href,
        style: { width: '110.8vw', top: '46.06vw', left: '-14.3vw' }
      },
      zat: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/zatmodel.webp', import.meta.url).href,
        style: { width: '93.13vw', top: '54.2vw', left: '6.3vw' }
      },
      kong: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/kongyolumodel.webp', import.meta.url).href,
        style: { width: '107vw', top: '51.65vw', left: '15.8vw' }
      },
      ivy: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/lucianmodel.webp', import.meta.url).href,
        style: { width: '88.2vw', top: '53.2vw', left: '10.18vw' }
      },
      drax: {
        src: new URL('../src/assets/img/Desktop/CHARACTER_WEBP/krysysmodel.webp', import.meta.url).href,
        style: { width: '46.05vw', top: '46.82vw', left: '29.5vw' }
      },
    };

    const backCoverSlotClass = (i) => {
      if (isAnimating.value) {
        if (i === prevIndex.value) {
          return direction.value === 'up' ? 'anim-up-out-delay' : 'anim-down-out-delay';
        }
        if (i === current.value) {
          return direction.value === 'up' ? 'anim-up-in-delay' : 'anim-down-in-delay';
        }
        return 'hidden-slot';
      }
      return i === current.value ? 'shown-slot' : 'hidden-slot';
    };

    const mModelStyleFor = (i) => {
      const c = mModelMap[slides[i].key] || {};
      return {
        ...c.style,
        transform: 'translate3d(0,0,0)',
      };
    };

    // Skills
    const mSkillMap = {
      yumi: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/yumiskills.webp', import.meta.url).href },
      zat: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/zatskills.webp', import.meta.url).href },
      kong: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/kongyoluskills.webp', import.meta.url).href },
      ivy: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/lucianskills.webp', import.meta.url).href },
      drax: { src: new URL('../src/assets/img/Mobile/CHARACTER_MOBILE_WEBP/krysusskill.webp', import.meta.url).href },
    };


    // Check when change width
    onMounted(() => {
      window.addEventListener("resize", handleResize);
      if (!isMobile.value) {
        initLenis();
      } else {
        destroyLenis();
      }
    });

    const currentKey = computed(() => slides[current.value].key);

    const actorSrc = computed(() => actorMap[currentKey.value]?.src || '');

    watch(isMobile, (val) => {
      if (val) {
        destroyLenis();
        document.body.style.overflow = 'auto';
      } else {
        initLenis();
        document.body.style.overflow = '';
      }
    });

    onBeforeUnmount(() => {
      window.removeEventListener("resize", handleResize);
      destroyLenis();
      if (lenis) {
        lenis.destroy();
      }
    });

    return {
      homeFrame,
      isMobile,
      gamePlay,
      initialIsMobile,
      adventure1,
      adventure2,
      adventure3,
      adventure4,
      adventure5,
      selectedIndex,
      selectThumb,
      basisStyle,
      imgStyle,
      ringClass,
      growStyle,
      secHome,
      secFeatures,
      secCharacters,
      secCampaign,
      secCommunity,
      secContact,
      scrollToRef,
      backGradient,
      line1Color,
      actorSrc,
      actorOffset,
      textOffset,
      next,
      prev,
      current,
      slides,
      // actorStyle,
      actorImages,
      cardSrc,
      cardStyle,
      wheelStyle,
      canPrev,
      canNext,
      actorWrapStyle,
      actorImgStyle,
      actorMap,
      prevIndex,
      direction,
      isAnimating,
      goTo,
      actorWrapStyleFor,
      actorImgStyleFor,
      actorSlotClass,
      glowColors,
      glowColor,
      STAGE_W,
      STAGE_H,
      backCoverWrapStyleFor,
      backCoverImgStyleFor,
      backCoverMap,
      revealMaskStyle,
      mCurrent,
      mCanPrev,
      mCanNext,
      mPrev,
      mNext,
      mStateClass,
      mBackgroundMap,
      mModelMap,
      mModelStyleFor,
      mSkillMap,
      backCoverSlotClass
    };
  },
  components: {
  },
  methods: {
    scrollTo(sectionId) {
      const element = document.getElementById(sectionId);
      if (!element) {
        console.warn(`Không tìm thấy phần tử với id: ${sectionId}`);
        return;
      }
      if (window.__lenis) {
        window.__lenis.scrollTo(element, { offset: 0 });
      } else {
        element.scrollIntoView({ behavior: "smooth" });
      }
    },
  },
}
</script>

<style>
@font-face {
  font-family: "Emeritus";
  src: url(../src/assets/fonts/Emeritus-Bold.ttf);
}

@font-face {
  font-family: "LeagueSpartan";
  src: url(../src/assets/fonts/LeagueSpartan-VariableFont_wght.ttf);
}

@font-face {
  font-family: "Inter";
  src: url(../src/assets/fonts/Inter-VariableFont_opsz,wght.ttf);
}

@font-face {
  font-family: "Lexend";
  src: url(../src/assets/fonts/Lexend-VariableFont_wght.ttf);
}


.font-emeritus {
  font-family: "Emeritus", sans-serif;
}

.font-league {
  font-family: "LeagueSpartan", sans-serif;
}

.font-inter {
  font-family: "Inter", sans-serif;
}

.font-lexend {
  font-family: "lexend", sans-serif;
}

body {
  background-color: #171717;
}

html,
body {
  height: auto;
}

@media (min-width: 769px) {
  body {
    overflow: hidden;
  }
}

@media (max-width: 768px) {
  body {
    overflow: auto;
  }
}

html {
  scrollbar-width: none;
}

html::-webkit-scrollbar {
  display: none;
}

.backdrop-blur-ip {
  backdrop-filter: blur(3vw);
  -webkit-backdrop-filter: blur(3vw);
}

.image-select-list {
  gap: 0.5vw;
  align-items: stretch;
}

.smooth-basis {
  flex: var(--g) 1 0%;
  min-width: 0;
  will-change: flex-grow;
  contain: layout paint;
  transition: flex-grow .45s cubic-bezier(.2, .7, .2, 1);
}

.thumb-img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
  transform: none !important;
  transition: filter .45s cubic-bezier(.2, .7, .2, 1);
}

.thumb {
  background: rgba(0, 0, 0, 0.02);
  overflow: hidden;
  height: 100%;
}

.abs-ring {
  position: absolute;
  inset: 0;
  border-radius: 0.8vw;
  outline: 2px solid transparent;
  transition: outline-color .45s;
}

.ring-on {
  outline-color: #F8B133;
}

.ring-off {
  outline-color: transparent;
}

.button-hover:hover .text-scale {
  transform: scale(1.2);
}

.button-hover:hover .overlay-hidden {
  opacity: 1;
}

.actor-rise-enter-from {
  transform: translate3d(0, 100%, 0);
  opacity: 0;
}

.actor-rise-enter-to {
  transform: translate3d(0, 0%, 0);
  opacity: 1;
}

.actor-rise-leave-from {
  transform: translate3d(0, 0%, 0);
  opacity: 1;
}

.actor-rise-leave-to {
  transform: translate3d(0, -100%, 0);
  opacity: 0;
}

.actor-rise-enter-active,
.actor-rise-leave-active {
  transition: transform 2s cubic-bezier(.22, 1, .36, 1), opacity 2s cubic-bezier(.22, 1, .36, 1);
  will-change: transform, opacity;
}

.actor-rise-enter-active {
  z-index: 2;
}

.actor-rise-leave-active {
  z-index: 1;
  position: absolute;
}

/* Optional: tôn trọng người dùng giảm chuyển động */
@media (prefers-reduced-motion: reduce) {

  .actor-rise-enter-active,
  .actor-rise-leave-active {
    transition-duration: .01ms !important;
  }
}

/* Base: slot ẩn mặc định */
.actor-slot {
  position: absolute;
}

/* Trạng thái nghỉ */
.shown-slot {
  display: block;
  opacity: 1;
  transform: none;
  z-index: 2;
}

.hidden-slot {
  display: none;
  opacity: 0;
  transform: translateY(100%);
  /* không quan trọng khi display:none */
}

/* Keyframes theo hướng */
@keyframes slideUpIn {
  from {
    transform: translateY(100%);
    opacity: 0;
  }

  to {
    transform: translateY(0);
    opacity: 1;
  }
}

@keyframes slideUpOut {
  from {
    transform: translateY(0);
    opacity: 1;
  }

  to {
    transform: translateY(-100%);
    opacity: 0;
  }
}

@keyframes slideDownIn {
  from {
    transform: translateY(-100%);
    opacity: 0;
  }

  to {
    transform: translateY(0);
    opacity: 1;
  }
}

@keyframes slideDownOut {
  from {
    transform: translateY(0);
    opacity: 1;
  }

  to {
    transform: translateY(100%);
    opacity: 0;
  }
}

/* Lớp animation áp cho 2 slot tham gia chuyển cảnh */
.anim-up-in,
.anim-up-out,
.anim-down-in,
.anim-down-out {
  display: block;
  /* phải hiện để animate */
  animation-duration: 1200ms;
  /* khớp ANIM_MS */
  animation-timing-function: cubic-bezier(.22, 1, .36, 1);
  animation-fill-mode: forwards;
  will-change: transform, opacity;
}

.anim-up-in {
  animation-name: slideUpIn;
  z-index: 2;
}

.anim-up-out {
  animation-name: slideUpOut;
  z-index: 1;
}

.anim-down-in {
  animation-name: slideDownIn;
  z-index: 2;
}

.anim-down-out {
  animation-name: slideDownOut;
  z-index: 1;
}

@media (prefers-reduced-motion: reduce) {

  .anim-up-in,
  .anim-up-out,
  .anim-down-in,
  .anim-down-out {
    animation-duration: .01ms !important;
  }
}

/* Cross-fade 0.7s cho 3 lớp: background / model / skill */
.m-layer {
  opacity: 0;
  visibility: hidden;
  transition: opacity 700ms ease, transform 700ms cubic-bezier(.2, .7, .2, 1);
  will-change: opacity, transform;
  pointer-events: none;
}

.m-show {
  opacity: 1;
  visibility: visible;
  transform: translate3d(0, 0, 0);
}

.m-hide {
  opacity: 0;
  visibility: hidden;
}

.model-img-mobile {}

.anim-up-in-delay {
  animation-name: slideUpIn;
  animation-duration: 1200ms;
  animation-timing-function: cubic-bezier(.22, 1, .36, 1);
  animation-fill-mode: forwards;
  will-change: transform, opacity;
  z-index: 2;
}

.anim-up-out-delay {
  animation-name: slideUpOut;
  animation-duration: 1200ms;
  animation-timing-function: cubic-bezier(.22, 1, .36, 1);
  animation-fill-mode: forwards;
  will-change: transform, opacity;
  z-index: 1;
}

.anim-down-in-delay {
  animation-name: slideDownIn;
  animation-duration: 1200ms;
  animation-timing-function: cubic-bezier(.22, 1, .36, 1);
  animation-fill-mode: forwards;
  will-change: transform, opacity;
  z-index: 2;
}

.anim-down-out-delay {
  animation-name: slideDownOut;
  animation-duration: 1200ms;
  animation-timing-function: cubic-bezier(.22, 1, .36, 1);
  animation-fill-mode: forwards;
  will-change: transform, opacity;
  z-index: 1;
}

.anim-up-in-delay,
.anim-up-out-delay,
.anim-down-in-delay,
.anim-down-out-delay {
  animation-duration: 1700ms;
}
</style>
