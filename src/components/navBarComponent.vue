<template>
  <nav
    class="absolute z-100 w-full h-12 sm:h-14 md:h-16 lg:h-20 text-white flex md:justify-around justify-between items-center"
  >
    <div class="md:p-0 px-12">
      <h1>شعار</h1>
    </div>
    <div class="">
      <!--burger icon-->
      <div>
        <button @click="toggleMenu" class="md:hidden text-white text-xl px-10">
          <font-awesome-icon icon="bars" class="text-2xl" />
        </button>

        <div
          :class="{
            'transform translate-x-0': isMenuOpen,
            'translate-x-full': !isMenuOpen,
          }"
          class="fixed top-0 right-0 z-50 w-64 h-full bg-slate-800 p-6 transition-transform duration-300 ease-in-out lg:hidden"
        >
          <button
            @click="toggleMenu"
            class="absolute top-4 right-4 text-white text-3xl"
          >
            <font-awesome-icon icon="times" />
          </button>

          <ul class="space-y-6">
            <li>
              <a href="/" @click="toggleMenu" class="text-white text-xl"
                >الرئيسية</a
              >
            </li>
            <li>
              <a
                href="#"
                @click="toggleMenu"
                class="text-white text-xl"
                @click.prevent="scrollToSection('about')"
                >عن الشركة</a
              >
            </li>
            <li>
              <a
                href="#"
                @click="toggleMenu"
                class="text-white text-xl"
                @click.prevent="scrollToSection('services')"
                >الخدمات</a
              >
            </li>
            <li>
              <a
                href="#"
                @click="toggleMenu"
                class="text-white text-xl"
                @click.prevent="scrollToSection('why-us')"
                >لماذا إمكان</a
              >
            </li>
            <li>
              <a
                href="#"
                @click="toggleMenu"
                class="text-white text-xl"
                @click.prevent="scrollToSection('contact-us')"
                >اتصل بنا</a
              >
            </li>
          </ul>
        </div>
      </div>
      <ul
        data-aos="fade-up"
        class="w-96 hidden md:flex md:flex-row-reverse md:justify-between"
      >
        <li><a href="/">الرئيسية</a></li>
        <li>
          <a href="#" @click.prevent="scrollToSection('about')">عن الشركة</a>
        </li>
        <li>
          <a href="#" @click.prevent="scrollToSection('services')">الخدمات</a>
        </li>
        <li>
          <a href="#" @click.prevent="scrollToSection('why-us')">لماذا إمكان</a>
        </li>
        <li>
          <a href="#" @click.prevent="scrollToSection('contact-us')"
            >اتصل بنا</a
          >
        </li>
      </ul>
    </div>
  </nav>
  <div class="">
    <img
      src="../assets/photo/Smart Home Appliances.jpg"
      class="sm:w-full sm:h-full h-80"
      alt="photo"
    />
    <div
      data-aos="fade-up"
      class="text-right absolute top-24 left-3 w-32 h-60 text-xs md:absolute md:top-1/3 md:left-20 md:w-96 md:h-60 text-white md:leading-relaxed md:text-xl"
    >
      مرحبًا بكم في إمكان للمباني الذكيه وتكنولوجيا المعلومات حيث المستقبل يبدأ
      من هنا! نحن في إمكان نؤمن بأن التكنولوجيا الذكية هي مفتاح الحياة العصرية
      المريحة والآمنة. نقدم حلولًا مبتكرة للتحكم في المنازل والمباني الذكية، مما
      يمنح عملاءنا تجربة فريدة تجمع بين الراحة، الأمان، والكفاءة في استهلاك
      الطاقة.
    </div>
  </div>
  <div class="mb-20">
    <svg
      width="100%"
      height="100%"
      viewBox="0 0 813 156"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <foreignObject x="0" y="0" width="0" height="0"
        ><div
          xmlns="http://www.w3.org/1999/xhtml"
          style="
            backdrop-filter: blur(2px);
            clip-path: url(#bgblur_0_32_3_clip_path);
            height: 100%;
            width: 100%;
          "
        ></div
      ></foreignObject>
      <g data-figma-bg-blur-radius="4">
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M0 156L34 141.109C68 126.927 136 97.8545 203 92.1818C271 86.5091 339 103.527 407 118.418C474 132.6 542 143.945 610 146.782C678 149.618 745 143.945 779 141.109L813 138.273V0H779C745 0 678 0 610 0C542 0 474 0 407 0C339 0 271 0 203 0C136 0 68 0 34 0H0V156Z"
          fill="#010251"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M0 156L34 141.109C68 126.927 136 97.8545 203 92.1818C271 86.5091 339 103.527 407 118.418C474 132.6 542 143.945 610 146.782C678 149.618 745 143.945 779 141.109L813 138.273V0H779C745 0 678 0 610 0C542 0 474 0 407 0C339 0 271 0 203 0C136 0 68 0 34 0H0V156Z"
          fill="#010251"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M0 156L34 141.109C68 126.927 136 97.8545 203 92.1818C271 86.5091 339 103.527 407 118.418C474 132.6 542 143.945 610 146.782C678 149.618 745 143.945 779 141.109L813 138.273V0H779C745 0 678 0 610 0C542 0 474 0 407 0C339 0 271 0 203 0C136 0 68 0 34 0H0V156Z"
          stroke="#070864"
        />
      </g>
      <defs>
        <clipPath id="bgblur_0_32_3_clip_path" transform="translate(0 0)">
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M0 156L34 141.109C68 126.927 136 97.8545 203 92.1818C271 86.5091 339 103.527 407 118.418C474 132.6 542 143.945 610 146.782C678 149.618 745 143.945 779 141.109L813 138.273V0H779C745 0 678 0 610 0C542 0 474 0 407 0C339 0 271 0 203 0C136 0 68 0 34 0H0V156Z"
          />
        </clipPath>
      </defs>
    </svg>
  </div>
</template>

<script setup>
import { ref } from "vue";
const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

const scrollToSection = (sectionId) => {
  const section = document.getElementById(sectionId);
  if (section) {
    section.scrollIntoView({ behavior: "smooth", block: "start" });
  }
};
</script>
