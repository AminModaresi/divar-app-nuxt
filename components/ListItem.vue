<template>
    <div class="grid grid-cols-12 gap-5">
        <div class="col-span-12 md:col-span-6" v-for="data in data.web_widgets.post_list" :key="data.data.token" :v-if="data.web_widgets">
            <ItemBox :title="data.data.title" :img="data.data.image_url ? data.data.image_url[0].src : ''" :bottom-description-text="data.data.bottom_description_text" :middle-description-text="data.data.middle_description_text"/>
        </div>
    </div>
</template>

<script setup>
    const {data, pending, error, refresh} = await useFetch("https://api.divar.ir/v8/web-search/mashhad")
</script>