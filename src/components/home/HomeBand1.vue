
<script>
import Button from '../reusable/Button.vue';
export default {
    components: { Button }
};
</script>

<template>

    <div class="flex justify-center bg-app-gray py-5">

        <p class="justify-center text-semibold text-lg pr-10">Pour vos tres prochaines consultations, notre equipe a votre disposition !</p>

        <div class="mr-5">
            <Button title="demander devis"
                class="border-2 border-main0 uppercase px-4 py-2 text-white font-bold tracking-wider bg-main0 hover:bg-main0 focus:ring-1 focus:ring-main0 duration-500"
                type="submit" aria-label="demander devis" />
        </div>

        <div>
            <Button title="nous visiter"
                class="uppercase px-4 py-2 text-main0 font-bold tracking-wider bg-app-gray border-2 border-main0"
                type="submit" aria-label="nous visiter" />
        </div>

    </div>

</template>