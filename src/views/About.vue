<script>
import AboutMe from '@/components/about/AboutMe';
import AboutCounter from '@/components/about/AboutCounter';
import AboutClients from '@/components/about/AboutClients';
// import CallToAction from '@/components/about/CallToAction';
import feather from 'feather-icons';

export default {
	name: 'About',
	components: {
		AboutMe,
		AboutCounter,
		AboutClients,
		// CallToAction,
	},
	data: () => {
		return {};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div>
	
		<div class="container mx-auto">
			<AboutMe />
		</div>

	
		<AboutCounter />

		
		<div class="container mx-auto">
			<AboutClients />
		</div>

		<!-- <CallToAction /> -->

	</div>
</template>

<style scoped></style>
