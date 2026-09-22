<script setup>
import messageImg from "@/assets/images/messages-section-img.jpg";
import { ArrowLeft, ArrowRight } from "@primeicons/vue";
</script>

<template>
  <div
    class="bg-gray-100 flex flex-col justify-center items-center gap-8 px-6 py-16 lg:px-0 lg:py-24"
  >
    <div class="flex flex-col gap-4 max-w-xl lg:max-w-3xl text-center">
      <h1
        class="text-3xl md:text-4xl lg:text-5xl font-bold tracking-tight leading-tight"
      >
        Messaging . Meetings . Collaboration
      </h1>
      <p class="text-md md:text-sm lg:text-lg">
        Aside providing the whole gamut for email messaging - SMTP, IMAP, POP3
        and friends - we are focussed on extending your collaboration needs with
        more productive apps.
      </p>
    </div>
    <div class="flex w-full items-center justify-center px-4 lg:gap-6 lg:px-0">
      <button
        class="hidden rounded-full bg-gray-100 p-4 transition-colors duration-500 ease-in-out hover:bg-gray-200 lg:block cursor-pointer"
      >
        <ArrowLeft />
      </button>

      <div
        class="flex w-full max-w-3xl flex-col overflow-hidden rounded-2xl bg-white lg:min-h-[700px] lg:max-w-6xl lg:flex-row"
      >
        <div
          class="flex w-full flex-col justify-between gap-8 px-4 py-6 lg:w-[30%] lg:gap-0 lg:px-4 lg:py-8"
        >
          <div class="flex flex-col gap-5 lg:gap-4">
            <div class="flex flex-col gap-1 px-2 lg:gap-2 lg:max-w-80">
              <h3 class="text-lg font-medium text-[#069] lg:text-2xl">Mail</h3>
              <p class="text-sm lg:text-lg">
                Fast, secure, and intuitive messaging for teams.
              </p>
            </div>

            <div class="flex flex-col gap-1 px-2 lg:gap-2 lg:max-w-80">
              <h3 class="text-lg font-medium text-[#069] lg:text-2xl">Chat</h3>
              <p class="text-sm lg:text-lg">
                Instant, reliable, and organized conversations that keep your
                team connected.
              </p>
            </div>

            <div class="flex flex-col gap-1 px-2 lg:gap-2 lg:max-w-80">
              <h3 class="text-lg font-medium text-[#069] lg:text-2xl">
                Contact
              </h3>
              <p class="text-sm lg:text-lg">
                A smarter way to manage and access all your professional
                connections in one place.
              </p>
            </div>
          </div>

          <div class="flex flex-wrap lg:flex-col gap-2 px-2">
            <div
              class="w-fit rounded-lg border border-gray-700/70 px-2 py-1 text-xs lg:text-sm"
            >
              Smart mail
            </div>
            <div
              class="w-fit rounded-lg border border-gray-700/70 px-2 py-1 text-xs lg:text-sm"
            >
              Instant Conversation
            </div>
            <div
              class="w-fit rounded-lg border border-gray-700/70 px-2 py-1 text-xs lg:text-sm"
            >
              Smart Connections
            </div>
          </div>
        </div>

        <div
          class="relative flex h-[360px] w-full items-end p-5 lg:h-auto lg:w-[70%] lg:p-10"
        >
          <img
            :src="messageImg"
            alt="Messaging image"
            class="absolute inset-0 h-full w-full object-cover"
          />

          <div
            class="relative z-10 flex w-full max-w-xs flex-col gap-4 lg:max-w-lg"
          >
            <h1
              class="text-2xl leading-none tracking-tight text-white lg:text-4xl"
            >
              Ration makes team conversations effortless, fast, secure, and
              always in sync.
            </h1>

            <button
              class="w-fit cursor-pointer rounded bg-white px-6 py-2 text-xs font-medium text-black transition-colors duration-300 ease-in-out hover:bg-gray-300 lg:text-sm"
            >
              Get Started
            </button>
          </div>
        </div>
      </div>

      <button
        class="hidden rounded-full bg-gray-100 p-4 transition-colors duration-500 ease-in-out hover:bg-gray-200 lg:block cursor-pointer"
      >
        <ArrowRight />
      </button>
    </div>
  </div>
</template>
