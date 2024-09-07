<script setup lang="ts">

const route = useRoute()

</script>


<template>
    <div class="flex flex-row items-center justify-between bg-white h-16 px-16">
        <NuxtLink
            to="/"
            class="font-bold"
        >
            LOGO
        </NuxtLink>
        <div class="flex flex-row gap-16">
            <div class="flex flex-col justify-center items-center">
                <NuxtLink
                    to="/"
                    :class="[route.name === 'index' ? 'text-primary-500' : 'text-black hover:text-primary-500', 'p-2 duration-300']"
                >
                    Accueil
                </NuxtLink>
                <span
                    :class="[route.name === 'index' ? 'w-[110%]' : 'w-0', 'h-0.5 bg-primary-500 duration-300 ease-in-out']"
                ></span>
            </div>
            <div class="flex flex-col justify-center items-center">
                <NuxtLink
                    to="/events"
                    :class="[route.name === 'events' ? 'text-primary-500' : 'text-black hover:text-primary-500', 'p-2 duration-300']"
                >
                    Évènements
                </NuxtLink>
                <span
                    :class="[route.name === 'events' ? 'w-[110%]' : 'w-0', 'h-0.5 bg-primary-500 duration-300 ease-in-out']"
                ></span>
            </div>
            <div class="flex flex-col justify-center items-center">
                <NuxtLink
                    to="/shop"
                    :class="[route.name === 'shop' ? 'text-primary-500' : 'text-black hover:text-primary-500', 'p-2 duration-300']"
                >
                    Boutique
                </NuxtLink>
                <span
                    :class="[route.name === 'shop' ? 'w-[110%]' : 'w-0', 'h-0.5 bg-primary-500 duration-300 ease-in-out']"
                ></span>
            </div>
        </div>
    </div>
</template>