<script>
import feather from 'feather-icons';
import FooterCopyright from './FooterCopyright.vue';


export default {
	components: { FooterCopyright },
	data() {
		return {

			navLink: [
				{
					id: 1,
					name: 'Notre Agence',
					url: '/about',
				},
				{
					id: 2,
					name: 'Notre Vision',
					url: '#',
				},
				{
					id: 3,
					name: 'Nos Secteurs',
					url: '#',
				},
				{
					id: 4,
					name: 'Nous Joindre',
					url: '/contact',
				},
			],

			serviceLink: [
				{
					id: 1,
					name: 'Training/Consulting',
					url: '/',
				},
				{
					id: 2,
					name: 'Communication',
					url: '#',
				},
				{
					id: 3,
					name: 'Gestion administrative',
					url: '#',
				},
				{
					id: 4,
					name: "Service d'envois",
					url: '/',
				},
				{
					id: 5,
					name: "Recrutement/Placement",
					url: '/',
				},
			],

			// socials: [
			// 	{
			// 		id: 1,
			// 		name: 'Facebook',
			// 		icon: 'facebook',
			// 		url: 'https://facebook.com/',
			// 	},
			// 	{
			// 		id: 2,
			// 		name: 'Twitter',
			// 		icon: 'twitter',
			// 		url: 'https://twitter.com/',
			// 	},
			// 	{
			// 		id: 4,
			// 		name: 'Instagram',
			// 		icon: 'instagram',
			// 		url: 'https://instagram.com/realstoman',
			// 	},
			// ],
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
};
</script>

<template>
	<div class="bg-app-gray mt-10">


		<div class="container mx-auto flex flex-col-reverse md:flex-row pt-5">

			<div class="w-full md:w-1/3">

				<div class="flex flex-col text-left mb-2">

					<p
						class="font-general-semibold uppercase text-2xl font-semibold text-primary-dark dark:text-primary-light mb-5">
						Qui sommes nous ?
					</p>

					<div class="">
						<img src="@/assets/images/logo-vect.png" class="w-26 h-16" alt="Logo" />
					</div>

					<div class="pt-2">
						<p>
							Incorporated Concept (Inc Concept) est une agence de prestation de services située à Ouagadougou, capitale politique du Burkina Faso. L’agence est animée par des équipes jeunes, dynamiques et compétentes dans un esprit d’innovation.
						</p>
					</div>

					<div class="pt-3 uppercase font-bold text-main0">
						<a href="/about">
							mieux nous connaitre
						</a>
					</div>

				</div>

			</div>

			<div class="w-full md:w-1/3">

				<div class="flex flex-col text-left mb-2 md:ml-10">
					<p
						class="font-general-semibold uppercase text-2xl font-semibold text-primary-dark dark:text-primary-light mb-5">
						Navigation
					</p>

					<div class="">

						<a v-for="item in navLink" :key="item.id" :href="item.url"
							class="hover:text-main0 dark:bg-ternary-dark duration-500">

							<ul class="text-left">
								<li class="pb-2 text-lg">
									{{ item.name }}
								</li>
							</ul>

						</a>

					</div>

				</div>

			</div>

			<div class="w-full md:w-1/3">

				<div class="flex flex-col text-left mb-2">
					<p
						class="font-general-semibold uppercase text-2xl font-semibold text-primary-dark dark:text-primary-light mb-5">
						nos services
					</p>

					<div class="">

						<a v-for="item in serviceLink" :key="item.id" :href="item.url"
							class="hover:text-main0 dark:bg-ternary-dark duration-500">

							<ul class="text-left">
								<li class="pb-2 text-lg">
									{{ item.name }}
								</li>
							</ul>

						</a>

					</div>

				</div>

			</div>

			<!-- <div class="w-full md:w-1/3">

					<div class="flex flex-col justify-center items-center mb-12 sm:mb-20">
						<p
							class="font-general-semibold text-2xl sm:text-2xl font-semibold text-primary-dark dark:text-primary-light mb-8">
							Nous suivre
						</p>
						
						<ul class="flex gap-4 sm:gap-8">
							<a v-for="social in socials" :key="social.id" :href="social.url" target="__blank"
								class="text-gray-400 hover:text-main0 dark:hover:text-main0 cursor-pointer rounded-full bg-gray-200 dark:bg-ternary-dark hover:bg-gray-200 shadow-sm p-3 duration-500">
								<i :data-feather="social.icon" class="w-4 h-4"></i>
							</a>
						</ul>

					</div>

				</div> -->

		</div>


		<FooterCopyright />

	</div>
</template>

<style scoped>
</style>
