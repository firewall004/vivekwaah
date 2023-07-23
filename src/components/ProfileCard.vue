<template>
  <div>
    <div class="h-24 w-full object-cover" />

    <div class="mx-auto max-w-5xl px-4 sm:px-6 lg:px-8">
      <div class="-mt-12 sm:-mt-16 sm:flex sm:items-end sm:space-x-5">
        <div class="flex">
          <img
            class="h-24 w-24 rounded-full ring-4 ring-white sm:h-32 sm:w-32"
            :src="profile.avatar"
            alt=""
          />
        </div>
        <div
          class="mt-4 sm:flex sm:min-w-0 sm:flex-1 sm:items-center sm:justify-end sm:space-x-6 sm:pb-1 mb-6"
        >
          <span class="relative inline-flex">
            <a
              type="button"
              :href="'mailto:' + profile.email"
              target="_blank"
              class="inline-flex items-center px-4 py-2 font-semibold leading-6 text-sm shadow rounded-md hover:text-gray-900 hover:bg-zinc-200 transition ease-in-out duration-75 ring-1 ring-slate-900/10 dark:ring-slate-200/20 delay-150 hover:-translate-y-1 hover:scale-110 bg-zinc-800 text-zinc-100 font-mono"
            >
              <EnvelopeIcon
                class="-ml-0.5 mr-1.5 h-5 w-5 text-yellow-600"
                aria-hidden="true"
              />
              Let's Talk
            </a>
            <span class="flex absolute h-3 w-3 top-0 right-0 -mt-1 -mr-1">
              <span
                class="animate-ping absolute inline-flex h-full w-full rounded-full bg-yellow-300 opacity-75"
              ></span>
              <span
                class="relative inline-flex rounded-full h-3 w-3 bg-yellow-500"
              ></span>
            </span>
          </span>
        </div>
      </div>
      <div class="mt-6 hidden min-w-0 flex-1 sm:block md:hidden">
        <h1 class="truncate text-2xl font-bold text-gray-900">
          {{ profile.name }}
        </h1>
      </div>
    </div>
  </div>
</template>

<script setup>
import { EnvelopeIcon } from "@heroicons/vue/20/solid";

const profile = {
  name: "Vivek Kumar",
  email: "kumar97vivek@yahoo.com",
  avatar:
    "https://media.licdn.com/dms/image/D4D35AQHAOA-8mA8xLA/profile-framedphoto-shrink_800_800/0/1689748479642?e=1690581600&v=beta&t=9KjKbvrgFsRT9JDYYGGZp_L7NrTzmSMMcb8kYgzZ4yQ",
  backgroundImage:
    "https://media.licdn.com/dms/image/C4D16AQFKAf_gKgPLGQ/profile-displaybackgroundimage-shrink_350_1400/0/1658518536241?e=1695254400&v=beta&t=c4TboWbqhd6E8uEugLJZRR0Jmcj8XKLbQ_Smi-ddx5g",
};
</script>
