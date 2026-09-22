<script setup>
import { ArrowRight, Database, Microphone, Users } from "@primeicons/vue";
import PricingCard from "@/components/PricingCard.vue";
import pricing from "@/pricing.json";
</script>

<template>
  <div
    class="bg-gray-100 flex items-center justify-center px-6 py-16 lg:px-0 lg:py-24"
  >
    <div
      class="w-full max-w-7xl flex flex-col items-center justify-center gap-8"
    >
      <div class="flex flex-col justify-center items-center gap-2">
        <h1
          class="text-3xl md:text-4xl lg:text-5xl font-bold tracking-tight text-center"
        >
          Pricing Plans
        </h1>
        <p class="font-medium text-center text-gray-500 max-w-xl lg:max-w-3xl">
          Start with collaboration. Do the work. Scale with confidence.
        </p>
        <div class="flex flex-col md:flex-row items-center gap-2">
          <p class="text-sm text-gray-500">Select your currency:</p>
          <select
            name="currency"
            id=""
            class="bg-gray-100 border border-gray-500 hover:bg-gray-200 px-2 py-1 transition-all duration-300 ease-in-out cursor-pointer"
          >
            <option value="" class="bg-white text-black">
              NGN - Nigeria Naira
            </option>
            <option value="" class="bg-white text-black">
              USD - American Dollar
            </option>
            <option value="" class="bg-white text-black">
              GBP - British Pound
            </option>
          </select>
        </div>
      </div>
      <div>
        <div class="flex flex-col items-center justify-center gap-4">
          <div
            class="w-fit flex items-center gap-2 bg-white border border-gray-200 rounded-full p-1"
          >
            <span class="bg-[#003854] text-white text-sm rounded-full px-4 py-2"
              >Monthly</span
            >
            <span class="pr-4"> Annual (save 2 months)</span>
          </div>
          <div class="flex flex-col lg:flex-row items-center gap-4">
            <PricingCard
              v-for="price in pricing.pricing"
              :key="price.id"
              :price="price"
            />
          </div>
          <p
            class="max-w-xl lg:max-w-3xl text-md md:text-sm text-center font-light mt-6"
          >
            All prices exclude VAT where applicable. Annual plans billed
            upfront. Savings calculated against monthly pricing. Fair usage
            limits apply to Ration Do and Ration Scale. 24/7 email support for
            all tiers. Priority support for Ration Scale.
          </p>
          <div
            class="flex flex-col justify-center items-center gap-6 lg:gap-4 mt-6"
          >
            <h2
              class="max-w-lg text-center text-3xl md:text-4xl lg:text-5xl font-medium"
            >
              Need more? Add what you need.
            </h2>
            <div class="flex flex-col md:flex-row items-center gap-4">
              <div
                class="w-full md:w-[220px] md:h-[240px] lg:w-[330px] lg:h-[220px] bg-white flex flex-col gap-2 rounded-xl shadow-xl px-6 py-4"
              >
                <Users class="text-[#069]" :size="35" />
                <h3 class="text-2xl font-bold tracking-tight mt-4">
                  Meeting Capacity
                </h3>
                <p class="text-gray-500 text-sm font-light">
                  Increase concurrent meetings & participant limits
                </p>
                <p
                  class="group flex items-center gap-2 text-[#069] font-semibold cursor-pointer mt-4"
                >
                  Contact Sales
                  <span
                    class="group-hover:translate-x-2 transition-all duration-500"
                    ><ArrowRight
                  /></span>
                </p>
              </div>
              <div
                class="w-full md:w-[220px] md:h-[240px] lg:w-[330px] lg:h-[220px] bg-white flex flex-col gap-2 rounded-xl shadow-xl px-6 py-4"
              >
                <Microphone class="text-[#069]" :size="35" />
                <h3 class="text-2xl font-bold tracking-tight mt-4">
                  Recording
                </h3>
                <p class="text-gray-500 text-sm font-light">
                  Meeting recording + cloud storage
                </p>
                <p class="font-medium pt-8">N500 / 10GB / month</p>
              </div>
              <div
                class="w-full md:w-[220px] md:h-[240px] lg:w-[330px] lg:h-[220px] bg-white flex flex-col gap-2 rounded-xl shadow-xl px-6 py-4"
              >
                <Database class="text-[#069]" :size="35" />
                <h3 class="text-2xl font-bold tracking-tight mt-4">
                  Extra Storage
                </h3>
                <p class="text-gray-500 text-sm font-light">
                  Additional Drive or Mailbox storage
                </p>
                <p class="font-medium pt-8">N300 / 10GB / month</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
