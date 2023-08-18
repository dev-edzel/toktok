<template>
    <div class="flex border-b py-6">
        <div class="cursor-pointer">
            <img class="rounded-full max-h-[60px]" width="60" src="https://socialcounts.org/_next/image?url=https%3A%2F%2Fwww.banner.yt%2FUCX8foYPDD2KVKhkGPpMSUCA%2Favatar%3Fwidth%3D640&w=256&q=75">
        </div>
        <div class="pl-3 w-full px-4">
            <div class="flex items-center justify-between pb-0.5">
                <button>
                    <span class="font-bold hover:underline cursor-pointer">
                        User name
                    </span>
                    <span class="text-[13px] text-light text-gray-500 pl-1 curson-pointer">
                        User name
                    </span>
                </button>
                <button class="border text-[15px] px-[21px] py-0.5 border-[#6654F4] text-[#6654F4] hover:bg-[#ffeef2] font-semibold rounded-md"> Follow </button>
            </div>
            <div class="text-[15px] pb-0.5 break-words md:max-w-[400px] max-w-[300px] ">
                Toktok
            </div>
            <div class="text-[14px] text-gray-500 pb-0.5"> #toktok #toktok #toktok </div>
            <div class="text-[14px] pb-0.5 flex items-center">
                <Icon name="mdi:music" size="17"/>
                <div class="px-1">original sound - TokTok</div>
                <Icon name="mdi:heart" size="20"/>
            </div>

            <div class="mt-2.5 flex">
                <div class="relative min-h-[480px] max-h-[580px] max-w-[260px] flex items-center bg-black rounded-xl cursor-point">
                    <video class="rounded-xl object-cover mx-auto h-full" src="~/assets/videos/toktok.mp4" ref="video" loop muted></video>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
let video = ref(null)

onMounted(() => video.value.play())
</script>
