<template>
  <div>
    <section class="flex items-center justify-between">
      <h1 class="text-[#0157AC] text-[32px] font-bold">Furnitures</h1>
      <div class="flex items-center justify-between gap-12">
        <div
          class="flex items-center rounded-[10px] h-[46px] w-[350px] bg-[#F4F3F9]"
        >
          <input
            class="w-full h-full bg-transparent outline-none px-5 placeholder:black/30 text-sm"
            placeholder="Qidirish..."
            type="text"
          />
          <img class="h-4 w-4 mr-5" src="@/assets/svg/search.svg" alt="" />
        </div>
        <button
          @click="store.filterModal = true"
          class="flex items-center justify-center bg-[#027DFC1A] rounded-[10px] h-[46px] w-[54px]"
        >
          <img src="@/assets/svg/filter.svg" alt="" />
        </button>
      </div>
    </section>
    <section>
      <ul class="flex items-center gap-8 mt-5 text-[24px] font-medium">
        <li class="flex items-center gap-2">
          <h1>Armchairs</h1>
          <p class="text-[#0157AC]">5</p>
        </li>
        <li class="flex items-center gap-2 text-black/40">
          <h1>Closets</h1>
          <p class="text-[#0157AC]">2</p>
        </li>
        <li class="flex items-center gap-2 text-black/40">
          <h1>Tables</h1>
          <p class="text-[#0157AC]">0</p>
        </li>
      </ul>
      <ul class="my-5">
        <li>
          <button
            class="flex items-center gap-3 h-8 px-4 rounded-full border border-[#0157AC] text-sm"
          >
            <p class="h-6 font-medium">Ijara uylar</p>
            <img src="@/assets/svg/blue_x.svg" alt="" />
          </button>
        </li>
      </ul>
    </section>
    <section>
      <!-- <Slider /> -->
      <div
        class="grid lg:grid-cols-4 md:grid-cols-3 sm:grid-cols-2 grid-cols-1 xl:gap-16 gap-5 -mx-[10px] mt-10"
      >
        <div
         @click="$router.push('/products/' + i)"
          v-for="i in 100"
          class="cursor-pointer bg-[#F8F8F8] max-w-[300px] h-[393px] p-[10px] rounded-2xl mx-auto"
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

    <!----------------------------------------------- filter --------------------------------------------------->
    <section>
      <el-drawer
        v-if="isMount"
        class="rounded-l-[40px] min-w-[500px] px-[30px] text-sm"
        v-model="store.filterModal"
        title="I am the title"
        :with-header="false"
      >
        <form @submit.prevent="store.filterModal = false">
          <div
            class="flex sticky top-0 h-[34px] items-center pt-[53px] justify-between bg-white"
          >
            <h1 class="font-medium text-2xl leading-7">Filters</h1>
            <img
              @click="store.filterModal = false"
              class="h-6 w-6 hover:bg-gray-200 rounded-md cursor-pointer"
              src="../../assets/svg/x.svg"
              alt="x"
            />
          </div>
          <div class="h-6 bg-white"></div>
          <div
            class="pt-[40px] space-y-[40px] pb-8 max-h-[calc(100vh_-_220px)] overflow-hidden overflow-y-auto"
          >
            <el-checkbox-group v-model="store.type">
              <el-checkbox label="All"
                ><p class="text-black ml-1 text-sm">All</p></el-checkbox
              >
              <el-checkbox label="Rent"
                ><p class="text-black ml-1 text-sm">For rent</p></el-checkbox
              >
              <el-checkbox label="Term"
                ><p class="text-black ml-1 text-sm">For term</p></el-checkbox
              >
              <el-checkbox label="Sale"
                ><p class="text-black ml-1 text-sm">For sale</p></el-checkbox
              >
            </el-checkbox-group>

            <div class="filterRequest">
              <h1 class="uppercase font-bold text-[11px]">FILTER BY PRICE</h1>
              <div class="flex items-center pt-4">
                <div class="relative">
                  <input
                    class="outline-none h-[46px] px-5 w-full text-center rounded-[10px] bg-[#F4F3F9]"
                    type="number"
                  />
                </div>
                <p class="px-[23px]">to</p>
                <div class="relative">
                  <input
                    class="outline-none h-[46px] px-5 w-full text-center rounded-[10px] bg-[#F4F3F9]"
                    type="number"
                  />
                </div>
              </div>
            </div>

            <div class="filterRequest">
              <h1 class="uppercase font-bold text-[11px]">
                FILTER BY CATEGORY
              </h1>
              <el-select
                v-model="store.categories"
                class="w-full py-3 mb-0.5"
                placeholder="Enter a category name ..."
                filterable
              >
                <el-option
                  v-for="item in ['Armchairs', 'Closets', 'Tables']"
                  @click="() => selectCategory(item)"
                  :key="item"
                  :label="item"
                  :value="item"
                  class="!bg-[#f4f3f9]"
                />
              </el-select>
              <div class="flex flex-wrap items-center gap-3">
                <div
                  class="flex items-center whitespace-nowrap justify-center gap-[10px] px-[14px] py-[8px] border border-[#027DFC] rounded-2xl h-8"
                >
                  <p>Armchairs</p>
                  <img
                    @click="() => closeShows(item.value)"
                    class="cursor-pointer -mr-2 hover:bg-gray-200 rounded-full p-1"
                    src="@/assets/svg/blue_x.svg"
                    alt=""
                  />
                </div>
                <div
                  class="flex items-center whitespace-nowrap justify-center gap-[10px] px-[14px] py-[8px] border border-[#027DFC] rounded-2xl h-8"
                >
                  <p>Closets</p>
                  <img
                    @click="() => closeShows(item.value)"
                    class="cursor-pointer -mr-2 hover:bg-gray-200 rounded-full p-1"
                    src="@/assets/svg/blue_x.svg"
                    alt=""
                  />
                </div>
              </div>
            </div>

            <div class="filterRequest">
              <h1 class="uppercase font-bold text-[11px]">FILTER BY COLORS</h1>
              <div class="flex items-center gap-2 h-[30px] mt-3">
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
          </div>

          <div class="absolute bottom-8 w-full bg-white pr-10 font-medium">
            <button
              @click="apply"
              class="h-[46px] w-[420px] text-white bg-[#027DFC] rounded-[10px]"
            >
              Apply filters
            </button>
            <button
              @click="clearFilters"
              class="h-[46px] w-[420px] text-[#027DFC] pt-8"
            >
              Clear all filters
            </button>
          </div>
        </form>
      </el-drawer>
    </section>
  </div>
</template>

<script setup>
const isMount = ref(false);
const store = reactive({
  filterModal: false,
  type: "All",
  categories: "",
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

onMounted(() => {
  isMount.value = true;
});
</script>
