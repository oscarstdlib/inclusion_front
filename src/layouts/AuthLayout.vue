<template>
    <div
        class="h-full h-screen flex flex-col sm:flex-row items-center md:items-start sm:justify-center md:justify-start flex-auto min-w-0">
        <div
            class="relative hidden md:flex flex-auto items-center justify-center w-1/2 h-full p-16 lg:px-28 overflow-hidden bg-gray-800 dark:border-r">
            <!-- Background - @formatter:off -->
            <!-- Rings -->
            <svg class="absolute inset-0 pointer-events-none" viewBox="0 0 960 540" width="100%" height="100%"
                preserveAspectRatio="xMidYMax slice" xmlns="http://www.w3.org/2000/svg">
                <g class="text-gray-700 opacity-25" fill="none" stroke="currentColor" stroke-width="100">
                    <circle r="234" cx="196" cy="23"></circle>
                    <circle r="234" cx="790" cy="491"></circle>
                </g>
            </svg>
            <!-- Dots -->
            <svg class="absolute -top-16 -right-16 text-gray-700" viewBox="0 0 220 192" width="220" height="192"
                fill="none">
                <defs>
                    <pattern id="837c3e70-6c3a-44e6-8854-cc48c737b659" x="0" y="0" width="20" height="20"
                        patternUnits="userSpaceOnUse">
                        <rect x="0" y="0" width="4" height="4" fill="currentColor"></rect>
                    </pattern>
                </defs>
                <rect width="220" height="192" fill="url(#837c3e70-6c3a-44e6-8854-cc48c737b659)"></rect>
            </svg>
            <!-- @formatter:on -->
            <!-- Content -->
            <div class="z-10 relative w-full max-w-2xl">
                <div class="text-7xl font-bold leading-none text-gray-100">
                    <!-- <div>Welcome to</div>
                    <div>our community</div> -->
                </div>
                <!-- <div class="mt-6 text-lg tracking-tight leading-6 text-gray-400">
                    Fuse helps developers to build organized and well coded dashboards full of beautiful and rich
                    modules.
                    Join us and start building your application today.
                </div> -->
               
            </div>
        </div>
        <div
            class="md:flex md:items-center md:justify-start w-full sm:w-auto md:h-full md:w-1/2 py-8 px-4 sm:p-12 md:p-16 sm:rounded-2xl md:rounded-none sm:shadow md:shadow-none sm:bg-card">
            <router-view></router-view>
        </div>
    </div>

</template>
<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>