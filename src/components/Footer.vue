<script setup>
import { Envelope, Facebook, Instagram, Linkedin, Twitter } from '@primeicons/vue';
import stackchaseLogo from "@/assets/images/stackchase-logo.png"
</script>

<template>
    <div class="w-full bg-white flex flex-col gap-10 py-20 px-40">
        <div class="flex justify-between">
            <div class="max-w-md flex flex-col gap-4">
                <img :src="stackchaseLogo" alt="Stackchase Logo" class="bg-black w-40">
                <p class="text-lg text-gray-500">
                    Stackchase Limited is a technology company building secure,
                    high-performance platforms that power modern collaboration, communication
                    and digital operations.
                </p>
            </div>
            <div class="flex gap-18">
                <div class="flex flex-col gap-4">
                    <h4 class="font-semibold">Company</h4>
                    <ol class="flex flex-col gap-1 text-gray-500">
                        <li class="hover:text-black cursor-pointer">About</li>
                        <li class="hover:text-black cursor-pointer">Product</li>
                        <li class="hover:text-black cursor-pointer">News</li>
                        <li class="hover:text-black cursor-pointer">Career</li>
                    </ol>
                </div>
                <div class="flex flex-col gap-4">
                    <h4 class="font-semibold">Industry</h4>
                    <ol class="flex flex-col gap-1 text-gray-500">
                        <li class="hover:text-black cursor-pointer">Government</li>
                        <li class="hover:text-black cursor-pointer">Business</li>
                    </ol>
                </div>
                <div class="flex flex-col gap-4">
                    <h4 class="font-semibold">Support</h4>
                    <ol class="flex flex-col gap-1 text-gray-500">
                        <li class="hover:text-black cursor-pointer">Product support</li>
                        <li class="hover:text-black cursor-pointer">Contact Us</li>
                    </ol>
                </div>
            </div>
        </div>
        <div class="flex justify-between text-gray-500 pt-6 border-t border-gray-200">
            <div class="flex gap-8">
                <p>© Copyright 2025 Stackchase Limited. All rights reserved.</p>
                <p class="hover:text-black cursor-pointer">Privacy policy</p>
                <p class="hover:text-black cursor-pointer">Legal notice</p>
                <p class="hover:text-black cursor-pointer">Feedback</p>
            </div>
            <div class="flex items-center gap-2">
                <Envelope class="hover:text-black cursor-pointer"/>
                <Facebook class="hover:text-black cursor-pointer"/>
                <Twitter class="hover:text-black cursor-pointer"/>
                <Linkedin class="hover:text-black cursor-pointer"/>
                <Instagram class="hover:text-black cursor-pointer"/>
            </div>
        </div>
    </div>
</template>