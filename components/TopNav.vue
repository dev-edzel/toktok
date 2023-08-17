<template>
    <div 
        id="TopNav" 
        class="fixed bg-white z-30 flex items-center w-full border-b h-[60px]">
        <div :class="route.fullPath === '/' ? 'max-w-[1150px]' : ''" class="flex items-center justify-between w-full px-6 mx-auto">
            <div :class="route.fullPath === '/' ? 'w-[80%]' : 'lg:w-[2%] w-[70%]'">
                <NuxtLink to="/">
                    <img width="115" src="~/assets/images/logo.png">
                </NuxtLink>
            </div>

            <div class="hidden md:flex items-center bg-[#F1F1F1] p-1 rounded-full max-w-[380px] w-full ">
                <input type="text" class="w-full pl-3 my-2 bg-transparent placeholder-[#838383] text-[15px] focus:outline-none" placeholder="Search Accounts">
            <div class="px-3 py-1 flex items-center border-l border-l-gray-300">
                <Icon name="ri-search-line" color="A1A2A7" size="22" /> 
            </div>
            </div>
            <div class="flex items-center justify-end gap-3 min-2-[275px] max-w-[320px] w-full">
                <button class="flex item-center border rounded-sm px-2 py-[6px] hover:bg-gray-100">
                    <Icon name="mdi:plus" color="#000000" size="22" />
                    <span class="px-2 font-medium text-[15px]"> Upload </span>
                </button>
            <div class="flex items-center">
                <button class="flex items-center bg-[#6654F4] text-white border rounded-md px-3 py-[6px]">
                    <span class="mx-4 font-medium text-[15px]">Log In</span>
                </button>
            </div>
            </div>
        </div>
    </div>
</template>

<script setup>
    const route = useRoute()
</script>
