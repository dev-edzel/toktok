<template>
    <div id="SideNavMain" :class="route.fullPath === '/' ? 'lg:w-[310px]' : 'lg:w-[220px]'" 
    class="fixed z-20 bg-white pt-[70px] h-full lg:border-r-0 border-r w-[75px] overflow-auto">
        <div class="lg:w-full w-[55px] mx-auto">
            <NuxtLink to="/">
                <MenuItem iconString="For You" colorString="#7060F1" sizeString="30"/>
            </NuxtLink>
            <MenuItem iconString="Following" colorString="#000000" sizeString="27"/>
            <MenuItem iconString="Live" colorString="#000000" sizeString="27"/>

            <div class="border-b lg:ml-2 mt-2" />
            
            <div class="lg:block hidden text-xs text-gray-600 font-semibold pt-4 pb-2 px-2">
                Suggested Accounts 
            </div>

            <div class="lg:hidden block pt-3" />

            <div class="cursor-pointer">
                <MenuItemFollow />
            </div>

            <button class="lg:block hidden text-[#6654F4] pt-1.5 pl-2 text-[13px]">
                See all
            </button>

            <div class="border-b lg:ml-2 mt-2" />

            <div class="lg:block hidden text-xs text-gray-600 font-semibold pt-4 pb-2 px-2">
                Following accounts
            </div>

            <div class="lg:hidden block pt-3" />

            <div class="cursor-pointer">
                <MenuItemFollow />
            </div>

            <button class="lg:block hidden text-[#6654F4] pt-1.5 pl-2 text-[13px]">
                See more
            </button>

            <div class="lg:block hidden border-b lg:ml-2 mt-2" />
            
            <div class="lg:block hidden text-[11px] text-gray-500 cursor-pointer">
                <div class="pt-4 px-2">Developers Transparency</div>
                <div class="pt-4 px-2">Help Safety Terms Privacy</div>
                <div class="pt-4 px-2">Creator Portal</div>
                <div class="pt-4 px-2">Community Guidelines</div>
                <div class="pt-4 px-2">© 2069 TokTok</div>
            </div>

            <div class="pb-14"></div>
        </div>
    </div>
</template>

<script setup>
const route = useRoute()
</script>

