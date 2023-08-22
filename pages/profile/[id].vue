<template>
    <MainLayout>
        <div class="pt-[90px] 2xl:pl-[185px] lg:pl-[160px] lg:pr-0 pr-2 w-[calc(100%-90px)] max-w-[1800px] 2xl:mx-auto">
            <div class="flex w-[calc(100vw-230px)]">
                <img class="max-w-[120px] rounded-full" src="https://socialcounts.org/_next/image?url=https%3A%2F%2Fwww.banner.yt%2FUCX8foYPDD2KVKhkGPpMSUCA%2Favatar%3Fwidth%3D640&w=256&q=75">
                <div class="ml-5 w-full">
                <div class="text-[30px] font-bold truncate">
                    User name
                </div>
                <div class="text-[18px] truncate">User name</div>
                <button v-if="true" class="flex item-center rounded-md py-1.5 px-3.5 mt-3 text-[15px] font-semibold border hover:bg-gray-100"> 
                    <Icon class="mt-0.5 mr-1" name="mdi:pencil" size="18" />
                    <div>Edit Profile</div>
                </button>
                <button v-else class="flex items-center rounded-md py-1.5 px-8 mt-3 text-[15px] text-white font-semibold bg-[#6654F4]">
                    Follow
                </button>
            </div>
            </div>
        </div>
    </MainLayout>
</template>

<script setup>
import MainLayout from '~/layouts/MainLayout.vue';
</script>
