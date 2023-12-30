<template>
  <main class="container mx-auto xl:px-28 md:px-10 px-5">
    <section class="flex md:flex-row flex-col gap-10 w-full">
      <!---------------------- carousel -------------------------->
      <div
        class="2xl:max-w-[522px] xl:max-w-[508px] lg:max-w-[452px] md:max-w-[324px] sm:max-w-[450px] max-w-[calc(100vw_-_40px)] w-full overflow-hidden"
      >
        <div
          class="flex max-w-[600px] bg-white rounded-xl duration-1000"
          id="carouselMain"
        >
          <img
            v-for="i in 5"
            :key="i"
            class="carouselImg bg-cover 2xl:min-w-[522px] xl:min-w-[508px] lg:min-w-[452px] md:min-w-[324px] sm:min-w-[450px] min-w-[calc(100vw_-_40px)] lg:h-[524px] md:h-[424px] bg-white object-contain rounded-2xl border border-gray-200 object-center"
            src="@/assets/images/furniture.png"
            alt=""
          />
        </div>
        <div id="carousel" class="grid grid-cols-5 w-full gap-[10px] mt-[10px]">
          <img
            id="img"
            v-for="(i, index) in 5"
            @click="store.slideStep = index + 1"
            :key="index"
            :class="store.slideStep == index + 1 ? 'border-black p-1' : ''"
            class="bottomIMages lg:h-[110px] md:h-[80px] sm:h-[110px] h-[150px] bg-white w-full cursor-pointer duration-500 object-contain border border-gray-200 rounded-lg"
            src="@/assets/images/furniture.png"
            alt=""
          />
        </div>
      </div>

      <!---------------------- carousel end -------------------------->

      <div class="w-full leading-10">
        <ul class="border-b-2 pb-6 mb-[3px] leading-[19px] space-y-6">
          <li
            class="flex leading-[19px] flex-wrap w-full justify-between font-semibold items-center"
          >
            <h2 class="font-semibold">#333014199</h2>
            <p class="flex items-center gap-3 cupoi">
              <img
                class="cursor-pointer md:h-6 duration-1000 md:w-6 h-4 w-4"
                src="@/assets/svg/like.svg"
                alt=""
              />
              Like
            </p>
          </li>
          <li class="leading-[19px] lg:text-2xl text-lg font-semibold">
            Buy our comfortable chair in every way 😍
          </li>
        </ul>
        <div>
          <h1>Colors:</h1>
          <div class="flex items-center gap-2 h-[30px]">
            <svg
              v-for="i in colors"
              width="30"
              height="30"
              viewBox="0 0 30 30"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="cursor-pointer"
            >
              <circle cx="15" cy="15" r="14.5" :fill="i" stroke="#E4E9F1" />
            </svg>
          </div>
        </div>
        <ul class="grid xl:grid-cols-4 lg:grid-cols-3 grid-cols-2 pt-2">
          <li>
            <h2>Price:</h2>
            <p class="font-bold">800 000 uzs</p>
          </li>
          <li>
            <h2>Quantity:</h2>
            <div
              class="flex items-center justify-around h-10 max-w-[120px] rounded-md overflow-hidden bg-[#EEEEEE] mt-1"
            >
              <button
                @click="() => changeQuantity('dec')"
                class="hover:bg-gray-200 h-full w-full"
              >
                <img class="mx-auto" src="@/assets/svg/minus.svg" alt="-" />
              </button>
              <p class="w-full text-center text-xl leading-6">
                {{ store.quantity }}
              </p>
              <button
                @click="() => changeQuantity('inc')"
                class="hover:bg-gray-200 h-full w-full"
              >
                <img class="mx-auto" src="@/assets/svg/plus.svg" alt="+" />
              </button>
            </div>
          </li>
        </ul>
        <div class="grid grid-cols-2 gap-5 my-8">
          <button
            class="md:text-md text-sm h-[50px] bg-[#027DFC] active:opacity-50 text-white font-semibold rounded-xl border border-[#027DFC]"
          >
            Add to Cart
          </button>
          <button
            class="md:text-md text-sm h-[50px] text-[#027DFC] active:opacity-50 rounded-xl font-semibold border border-[#027DFC]"
          >
            Buy in a click
          </button>
        </div>
      </div>
    </section>
    <section class="mt-20">
      <h1 class="text-[28px]">The latest ones</h1>
      <div class="flex items-center gap-5 mt-6 overflow-y-auto">
        <div
          v-for="i in 10"
          class="bg-[#F8F8F8] min-w-[300px] h-[393px] p-[10px] rounded-2xl"
        >
          <img
            class="rounded-[12px] w-[279px] h-[282px] object-cover"
            src="@/assets/images/furniture.png"
            alt=""
          />
          <ul class="flex items-center gap-8 my-[10px] h-4 text-sm font-medium">
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/heart.svg" alt="" />
              <p>16</p>
            </li>
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/watched.svg" alt="" />
              <p>16</p>
            </li>
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/comment.svg" alt="" />
              <p>16</p>
            </li>
          </ul>
          <h1 class="text-lg font-bold leading-4 mb-[10px]">
            Richmond Appartment
          </h1>
          <ul class="flex items-center justify-between">
            <li class="text-lg font-bold">$985,000</li>
            <li class="flex items-center gap-3">
              <img src="@/assets/svg/heart_white.svg" alt="" />
              <img src="@/assets/svg/cart.svg" alt="" />
            </li>
          </ul>
        </div>
      </div>
    </section>
    <section class="mt-10">
      <h1 class="text-[28px]">Similar ones</h1>
      <div class="flex items-center gap-5 mt-6 overflow-y-auto">
        <div
          v-for="i in 10"
          class="bg-[#F8F8F8] min-w-[300px] h-[393px] p-[10px] rounded-2xl"
        >
          <img
            class="rounded-[12px] w-[279px] h-[282px] object-cover"
            src="@/assets/images/furniture.png"
            alt=""
          />
          <ul class="flex items-center gap-8 my-[10px] h-4 text-sm font-medium">
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/heart.svg" alt="" />
              <p>16</p>
            </li>
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/watched.svg" alt="" />
              <p>16</p>
            </li>
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/comment.svg" alt="" />
              <p>16</p>
            </li>
          </ul>
          <h1 class="text-lg font-bold leading-4 mb-[10px]">
            Richmond Appartment
          </h1>
          <ul class="flex items-center justify-between">
            <li class="text-lg font-bold">$985,000</li>
            <li class="flex items-center gap-3">
              <img src="@/assets/svg/heart_white.svg" alt="" />
              <img src="@/assets/svg/cart.svg" alt="" />
            </li>
          </ul>
        </div>
      </div>
    </section>

    <Footer />
  </main>
</template>

<script setup>
const store = reactive({
  slideStep: 1,
  quantity: 1,
});

const colors = [
  "#FFF",
  "#0094FF",
  "#00FF57",
  "#FFEC40",
  "#FF002E",
  "#FF3C99",
  "#9919D6",
  "#A86060",
  "#FF9C40",
  "#939393",
];

function changeQuantity(type) {
  if (type == "inc") {
    store.quantity += 1;
  } else if (type == "dec") {
    if (store.quantity > 1) {
      store.quantity -= 1;
    }
  }
}

watch(
  () => store.slideStep,
  () => {
    document.getElementById("carouselMain").style.transform = `translateX(-${
      store.slideStep * 100 - 100
    }%)`;
  }
);
</script>

<style lang="scss" scoped>
input:focus {
  outline: none !important;
  outline: 0 !important;
}

.ul {
  list-style-type: disc;
}

@media (max-width: 500px) {
  .bottomIMages {
    height: 120px;
  }
}

@media (max-width: 450px) {
  .carouselImg {
    height: 450px;
  }
  .bottomIMages {
    height: 100px;
  }
}

@media (max-width: 400px) {
  .carouselImg {
    height: 400px;
  }
  .bottomIMages {
    height: 80px;
  }
}

@media (max-width: 350px) {
  .carouselImg {
    height: 350px;
  }
}
</style>
