<template>
    <div class="rounded flex p-4 bg-white h-[168px] shadow">
        <div class="ml-5 flex-[0_0_136px] h-[136px] rounded overflow-hidden">
            <img class="h-full w-full" :src="img" :alt="title" v-if="img">
            <div class="flex justify-center items-center h-full w-full bg-gray-200 text-[3rem] text-gray-500" v-else>
                <Icon name="ri:camera-off-fill" />
            </div>
        </div>
        <div class="flex flex-1 flex-col h-full justify-between">
            <p>{{ title }}</p>
            <div>
                <p class="text-sm mb-2">
                    {{ middleDescriptionText }}
                </p>
                <p class="text-[.7rem]">
                    {{ bottomDescriptionText }}
                </p>
            </div>
        </div>
    </div>
</template>
<script setup>
    const props = defineProps(["title" , "img" , "bottomDescriptionText" , "middleDescriptionText"])
</script>