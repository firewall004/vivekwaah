<template>
  <div class="h-screen">
    <main>
      <div class="mx-auto w-full">
        <profile-card />
      </div>
      <div class="relative isolate px-6 lg:px-8 select-none">
        <div class="mx-auto pt-16 pb-4 sm:pt-32 sm:pb-60">
          <div class="text-center">
            <div class="flex items-center justify-center">
              <div class="w-max">
                <h1
                  class="mb-2 overflow-hidden font-mono text-4xl dark:text-gray-400 md:text-6xl"
                >
                  Hi<span class="text-yellow-700">,</span> I<span
                    class="text-yellow-700"
                    >'</span
                  >m <br class="block md:hidden" />
                  <span class="relative">
                    <span
                      class="overflow-x-hidden whitespace-nowrap pt-2 text-brand-accent text-yellow-700"
                    >
                      vivek <span class="text-3xl md:text-5xl">👋</span>
                    </span>
                    <span
                      class="absolute -bottom-0 -top-1 left-0 inline-block w-full animate-type bg-white will-change-transform [font-family:monospace] after:absolute after:block after:h-full after:w-2 after:animate-cursor after:bg-zinc-900 after:content-[''] dark:bg-zinc-900 after:dark:bg-gray-100"
                    ></span>
                  </span>
                </h1>
              </div>
            </div>
            <p
              class="mt-6 text-lg leading-8 text-gray-500 font-mono tracking-wide brightness-100 scale-150"
            >
              {{ '<Web Developer />' }}
            </p>
            <p class="mt-16 text-lg leading-8 text-gray-500 font-mono">
              Passionate about clean and elegant code, dedicated to delivering
              seamless user experiences
            </p>
          </div>
        </div>
      </div>
    </main>
    <app-footer />
  </div>
</template>

<script setup>
import ProfileCard from "@/components/ProfileCard.vue";
import AppFooter from "@/components/common/AppFooter.vue";
</script>

<style scoped>
.cursor::after {
  display: block;
  content: "";
  position: absolute;
  width: 4px;
  height: 100%;
  background-color: #fff;
  animation: cursor 0.6s linear infinite alternate;
  will-change: opacity;
}

@keyframes cursor {
  0%,
  40% {
    opacity: 1;
  }

  60%,
  100% {
    opacity: 0;
  }
}
</style>
