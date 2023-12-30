<template>
  <div class="container mx-auto xl:px-28 md:px-10 px-5 bg-white flex flex-col pb-11 max-md:px-5">
    <div
      class="border bg-white self-center flex w-full flex-col items-stretch mt-5 pb-7 rounded-md border-solid border-neutral-200 max-md:max-w-full"
    >
      <img data-aos="fade-up"
        loading="lazy"
        src="@/assets/images/user_image.png"
        class="aspect-[3.99] object-contain object-center w-full overflow-hidden max-md:max-w-full"
      /><img data-aos="fade-down"
        loading="lazy"
        src="@/assets/images/user.png"
        class="aspect-square object-contain object-center md:w-[170px] sm:w-[120px] md:-mt-[85px] sm:-mt-[60px] w-[100px] -mt-[50px] overflow-hidden self-center z-[1] max-w-full"
      />
      <div data-aos="fade-up"
        class="z-[1] flex w-[409px] max-w-full flex-col items-stretch ml-6 -mt-3.5 self-start max-md:ml-2.5"
      >
        <div class="text-neutral-900 text-2xl font-medium">John Doe</div>
        <div class="text-neutral-900 text-sm leading-5 mt-2">IT Specialist</div>
        <div class="text-neutral-900 text-sm leading-5 mt-2">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed dapibus
          eros eu vehicula interdum.
        </div>
        <div class="items-stretch flex gap-2 mt-11 max-md:mt-10">
          <button
            class="border flex justify-between items-center gap-1 px-4 rounded-full border-solid border-sky-600"
          >
            <img
              loading="lazy"
              src="@/assets/svg/send.svg"
              class="aspect-[1.33] object-contain object-center w-4 stroke-[1.5px] stroke-sky-600 overflow-hidden shrink-0 max-w-full"
            />
            <div class="text-sky-600 mb-1 text-sm font-semibold leading-5">
              send a message
            </div>
          </button>
          <button
            class="text-zinc-600 text-sm font-semibold leading-5 border justify-center items-stretch px-5 h-8 rounded-full border-solid border-zinc-600"
          >
            More
          </button>
        </div>
      </div>
    </div>
    <div
      class="border bg-white self-center flex w-full flex-col mt-2 pl-6 pr-20 py-7 rounded-md border-solid border-neutral-200 items-start max-md:max-w-full max-md:px-5"
    >
      <div data-aos="fade-up" class="text-neutral-900 text-lg font-medium">Contact here</div>
      <div class="flex">
        <div class="flex flex-col min-w-[24px] w-6 items-center gap-2 mt-6">
          <img data-aos="fade-up" src="@/assets/svg/phone.svg" alt="" />
          <img data-aos="fade-up" src="@/assets/svg/telegram.svg" alt="" />
          <img data-aos="fade-up" src="@/assets/svg/instagram.svg" alt="" />
          <img data-aos="fade-up" src="@/assets/svg/youtube.svg" alt="" />
          <img data-aos="fade-up" src="@/assets/svg/location.svg" alt="" />
        </div>
        <div>
          <div data-aos="fade-up" class="flex items-center gap-1.5 ml-2 mt-7 max-md:ml-2.5">
            <p class="text-black text-xs whitespace-nowrap my-auto">
              +92 1234567890
            </p>
            <img loading="lazy" src="@/assets/svg/watched.svg" class="w-4" />
          </div>
          <p data-aos="fade-up"
            class="text-black text-xs whitespace-nowrap ml-2 mt-3 max-md:ml-2.5"
          >
            @gmail
          </p>
          <p data-aos="fade-up"
            class="text-black text-xs whitespace-nowrap ml-2 mt-4 max-md:ml-2.5"
          >
            @gmail
          </p>
          <p data-aos="fade-up"
            class="text-black text-xs whitespace-nowrap ml-2 mt-4 max-md:ml-2.5"
          >
            @gmail
          </p>
          <p data-aos="fade-up" class="text-black text-xs ml-2 mt-4 max-md:ml-2.5">
            Street 2, house #05, Motarway Route Road Islamabad, Pakistan
          </p>
        </div>
      </div>
    </div>
    <div
      class="border bg-white self-center flex w-full flex-col mt-2 pt-7 pb-4 px-7 rounded-md border-solid border-neutral-200 max-md:max-w-full max-md:px-5"
    >
      <h1 class="text-neutral-900 text-lg font-medium whitespace-nowrap">
        Experiences
      </h1>
      <div data-aos="fade-up" v-for="i in 5" class="border-b max-md:max-w-full">
        <div
          class="gap-5 mt-4 flex"
        >
          <div class="sm:flex">
            <img
              loading="lazy"
              src="@/assets/images/Group.png"
              class="object-cover w-[100px] h-[96px] rounded-2xl overflow-hidden self-center"
            />
            <div
              class="flex flex-col w-[82%] sm:ml-5 sm:mt-0 mt-3"
            >
              <div class="flex grow flex-col max-md:max-w-full">
                <div
                  class="text-neutral-900 text-sm font-semibold leading-5 self-stretch max-md:max-w-full"
                >
                  Freelance UX/UI designer
                </div>
                <div
                  class="text-neutral-900 text-xs font-medium leading-4 self-stretch mt-1 max-md:max-w-full"
                >
                  Lorem ipsum
                </div>
                <div class="flex gap-5 mt-0.5 self-start items-start">
                  <div
                    class="text-neutral-900 text-xs leading-4 grow whitespace-nowrap"
                  >
                    Jun 2022 — Present
                  </div>
                  <div
                    class="text-sky-600 text-xs font-semibold leading-4 self-stretch grow whitespace-nowrap"
                  >
                    1 yrs 02 mos
                  </div>
                </div>
                <div
                  class="text-neutral-900 text-xs leading-4 self-stretch mt-2 max-md:max-w-full"
                >
                  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed
                  dapibus eros eu vehicula interdum. Cras nec ultricies massa.
                  Curabitur rutrum, diam id consequat consequat
                </div>
              </div>
            </div>
          </div>
        </div>
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
      </div>

      <div class="self-center flex items-stretch gap-2.5 mt-4">
        <div
          class="text-neutral-400 text-sm font-medium grow whitespace-nowrap"
        >
          Show more
        </div>
        <div
          class="text-sky-500 text-sm font-medium whitespace-nowrap self-start"
        >
          25
        </div>
      </div>
    </div>
    <Footer />

  </div>
</template>
