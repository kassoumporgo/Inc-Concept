<script>
import AppBanner from '@/components/shared/AppBanner';
// import ProjectsGrid from '../components/projects/ProjectsGrid.vue';
// import Button from '../components/reusable/Button.vue';
import HomeBand1 from '../components/home/HomeBand1.vue';
import HomeBand2 from '../components/home/HomeBand2.vue';
import HomeClient from '../components/home/HomeClients.vue';
import HomeContent1 from '../components/home/HomeContent1.vue';
// import HomeContent2 from '../components/home/HomeContent2.vue';

export default {
	name: 'Home',
	components: {
		AppBanner,
		// ProjectsGrid,
		// Button,
		HomeBand1,
		HomeBand2,
		HomeClient,
		HomeContent1,
		// HomeContent2,
	},
};
</script>

<template>
	<div class="">

		<AppBanner class="mb-5 sm:mb-8" />

		<HomeBand1 />

		<HomeContent1/>

		<!-- <HomeContent2/> -->

		<!-- <div class="container mx-">

			<ProjectsGrid />

			<div class="mt-10 sm:mt-20 flex justify-center">
				<router-link to="/projects"
					class="font-general-medium flex items-center px-6 py-3 rounded-lg shadow-lg hover:shadow-xl bg-indigo-500 hover:bg-indigo-600 focus:ring-1 focus:ring-indigo-900 text-white text-lg sm:text-xl duration-300"
					aria-label="More Projects">
					<Button title="Toutes les réalisations" />
				</router-link>
			</div>

		</div> -->

		<HomeBand2 />

		<HomeClient />

	</div>
</template>

<style scoped>
</style>
