<template>
  <div>
    <div>
      <img
        class="h-32 w-full object-cover lg:h-48"
        :src="profile.backgroundImage"
        alt=""
      />
    </div>
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
          class="mt-6 sm:flex sm:min-w-0 sm:flex-1 sm:items-center sm:justify-end sm:space-x-6 sm:pb-1"
        >
          <div class="mt-6 min-w-0 flex-1 sm:hidden md:block">
            <h1 class="truncate text-2xl font-bold text-gray-900">
              {{ profile.name }}
            </h1>
          </div>
          <div
            class="mt-6 flex flex-col justify-stretch space-y-3 sm:flex-row sm:space-x-4 sm:space-y-0"
          >
            <a
              type="button"
			  href="mailto:{{ email }}"
			  target="_blank"
              class="inline-flex justify-center rounded-md bg-white px-3 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50"
            >
              <EnvelopeIcon
                class="-ml-0.5 mr-1.5 h-5 w-5 text-gray-400"
                aria-hidden="true"
              />
              <span>Message</span>
            </a>
          </div>
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
import { EnvelopeIcon, PhoneIcon } from "@heroicons/vue/20/solid";

const profile = {
  name: "Vivek Kumar",
  email: "kumar97vivek@yahoo.com",
  avatar:
    "https://media.licdn.com/dms/image/D4D35AQHAOA-8mA8xLA/profile-framedphoto-shrink_800_800/0/1689748479642?e=1690581600&v=beta&t=9KjKbvrgFsRT9JDYYGGZp_L7NrTzmSMMcb8kYgzZ4yQ",
  backgroundImage:
    "https://media.licdn.com/dms/image/C4D16AQFKAf_gKgPLGQ/profile-displaybackgroundimage-shrink_350_1400/0/1658518536241?e=1695254400&v=beta&t=c4TboWbqhd6E8uEugLJZRR0Jmcj8XKLbQ_Smi-ddx5g",
};
</script>
