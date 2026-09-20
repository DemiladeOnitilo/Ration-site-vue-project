<script setup>
import messageImg from "@/assets/images/messages-section-img.jpg";
import { ArrowLeft, ArrowRight } from "@primeicons/vue";
</script>

<template>
  <div
    class="bg-gray-100 flex flex-col justify-center items-center gap-8 py-24"
  >
    <div class="flex flex-col gap-4 max-w-3xl text-center">
      <h1 class="text-5xl font-bold tracking-tight leading-tight">
        Messaging . Meetings . Collaboration
      </h1>
      <p class="text-lg">
        Aside providing the whole gamut for email messaging - SMTP, IMAP, POP3
        and friends - we are focussed on extending your collaboration needs with
        more productive apps.
      </p>
    </div>
    <div class="w-full flex justify-center items-center gap-6">
      <button
        class="bg-gray-200 hover:bg-gray-300 p-4 rounded-full transition-color duration-500 ease-in-out cursor-pointer"
      >
        <ArrowLeft />
      </button>

      <div class="w-full max-w-6xl flex ">
        <div
          class="bg-white w-[20%] min-h-[700px] flex flex-col justify-between px-4 py-8 rounded-l-2xl"
        >
          <div class="flex flex-col gap-4">
            <div class="flex flex-col gap-2 w-full max-w-60 px-2">
              <h3 class="text-2xl text-[#069] font-medium">Mail</h3>
              <p>Fast, secure, and intuitive messaging for teams.</p>
            </div>
            <div class="flex flex-col gap-2 w-full max-w-60 px-2">
              <h3 class="text-2xl text-[#069] font-medium">Chat</h3>
              <p>
                instant, reliable, and organized conversations that keep your
                team connected.
              </p>
            </div>
            <div class="flex flex-col gap-2 w-full max-w-60 px-2">
              <h3 class="text-2xl text-[#069] font-medium">Contact</h3>
              <p>
                A smarter way to manage and access all your professional
                connection in one place.
              </p>
            </div>
          </div>

          <div class="flex flex-col gap-1 px-2">
            <div
              class="w-fit text-sm border border-gray-700/70 rounded-lg py-1 px-2"
            >
              Smart mail
            </div>
            <div
              class="w-fit text-sm border border-gray-700/70 rounded-lg py-1 px-2"
            >
              Instant Conversation
            </div>
            <div
              class="w-fit text-sm border border-gray-700/70 rounded-lg py-1 px-2"
            >
              Smart Connections
            </div>
          </div>
        </div>
        <div class="relative min-h-[700px] w-[80%] p-10 flex items-end">
          <img
            :src="messageImg"
            alt="messaging image"
            class="absolute inset-0 w-full h-full object-full rounded-r-2xl"
          />
          <div class="relative z-10 w-full max-w-lg flex flex-col gap-4">
            <h1 class="text-white text-4xl">
              Ration makes team conversations effortless, fast, secure, and
              always in sync.
            </h1>
            <button
              class="w-fit bg-white hover:bg-gray-300 text-black text-sm font-medium px-6 py-2 rounded transition-colors duration-300 ease-in-out cursor-pointer"
            >
              Get Started
            </button>
          </div>
        </div>
      </div>

      <button
        class="bg-gray-200 hover:bg-gray-300 p-4 rounded-full transition-color duration-500 ease-in-out cursor-pointer"
      >
        <ArrowRight />
      </button>
    </div>
  </div>
</template>
