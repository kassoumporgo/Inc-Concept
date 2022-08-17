<script>

import services from '../../data/services.js';


export default {

    data: () => {
        return {
            services,
        };
    },

};

</script>


<template>

    <div class="bg-app-black-1 py-5">

        <div v-for="item in services" :key="item.id" class="inline">

            <span class="uppercase font-bold text-white p-2.5 border-2 m-2">
                <a href="">{{ item.title }}</a>
            </span>

        </div>


    </div>

</template>