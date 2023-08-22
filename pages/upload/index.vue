<template>
        <UploadLayout>
            <div class="w-full mt-[80px] mb-[40px] bg-white shadow-lg rounded-md py-6 md:px-10 px-4">
                <div>
                    <div class="text-[23px] font-semibold">Upload Video</div>
                    <div class="text-gray-400 mt-1">Post Video </div>
                </div>

                <div class="mt-8 md:flex gap-6">
                    <label v-if="false" for="fileInput" class="md:mx-0 mx-ato mt-4 mb-6 flex flex-col items-center justify-center w-full max-w-[260px] h-[470px] text-center p-3 border-2 border-dashed border-gray-300 rounded-lg hover:bg-gray-100 cursor-pointer">
                        <Icon name="majesticons:cloud-upload" size="50" color="b3b3b1"></Icon>
                        <div class="mt-4 text-[17px]">Select video to upload</div>
                        <div class="mt-1.5 text-gray-500 text-[13px]">Drag and drop files</div>
                        <div class="mt-1.5 text-gray-500 text-[13px]">Long videos can be split into multiple parts to get more exposure</div>
                        <div class="mt-12 text-gray-400 text-sm">Support mp4</div>
                        <div class="mt-1 text-gray-400 text-[13px]">Up to 600 seconds</div>
                        <div class="mt-1 text-gray-400 text-[13px]">Less than 2 GB</div>
                        <div class="mt-1 text-gray-400 text-[13px]">Less than 30 videos</div>
                        <div class="px-2 py-1.5 mt-8 text-white text-[15px] w-[80%] bg-[#6654F4] rounded-sm"> Select files</div>
                        <input ref="file" type="file" id="fileInput" hidden accept=".mp4">
                    </label>
                    <div v-else class="md:mx-0 mx-auto mt-4 md:mb-12 mb-16 flex items-center justify-center w-full max-w-[260px] h-[540px] p-3 rounded-2xl cursor-pointer relative">
                        <div class="bg-black h-full w-full" />

                        <img class="absolute z-20 pointer-events-none" src="~/assets/images/mobile-case.png">
                        <video autoplay loop muted src="~/assets/videos/toktok.mp4" height="100"></video>
                        <div class="absolute -bottom-12 flex items-center justify-between z-50 rounded-xl border w-full p-2 border-gray-300">
                            <div class="flex  items-center truncate">
                                <Icon name="clarity:success-standard-line" size="16" class="min-w-[16px]" />
                                <div class="text-[11px] pl-1 truncate text-ellipsis">video name</div>
                            </div>
                            <button class="text-[11px] ml-2 font-semibold"> Change </button>
                        </div>
                    </div>

                    <div class="mt-4 mb-6">
                        <div class="flex bg-[#F8F8F8] py-4 px-6">
                            <div>
                                <Icon class="mr-4" size="20" name="mdi:box-cutter-off" />
                            </div>
                            <div>
                                <div class="text-sembold text-[15px] mb-1.5">Divide videos and edit</div>
                                <div class="text-semibold text-[13px] text-gray-400">Divide</div>
                            </div>
                        </div>
                        <div class="flex justify-end max-w-[130px] w-full h-full text-center my-auto">
                            <button class="px-8 py-1.5 text-white text-[15px] bg-[#6654F4] rounded-sm"> Edit </button>
                        </div>  
                    </div>
                </div> 
            </div>
        </UploadLayout>
</template>

<script setup>
import UploadLayout from '~/layouts/UploadLayout.vue';
</script>
