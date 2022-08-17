
<script>
export default {
	data: () => {
		return {
			copyrightDate: new Date().getFullYear(),
			projectName: 'Inc Concept',
			author: 'Kassoum',

			socials: [
				{
					id: 1,
					name: 'Facebook',
					icon: 'facebook',
					url: 'https://facebook.com/',
				},
				{
					id: 2,
					name: 'Twitter',
					icon: 'twitter',
					url: 'https://twitter.com/',
				},
				{
					id: 4,
					name: 'Instagram',
					icon: 'instagram',
					url: 'https://instagram.com/realstoman',
				},
			],

		};
	},
};
</script>


<template>
	<div class="justify-center items-center text-center pb-3">

		<div class="flex justify-center pb-5">
			<ul class="flex gap-4 sm:gap-8">
				<a v-for="social in socials" :key="social.id" :href="social.url" target="__blank"
					class="text-gray-400 hover:text-main0 dark:hover:text-main0 cursor-pointer rounded-full bg-gray-200 dark:bg-ternary-dark hover:bg-gray-200 shadow-sm p-3 duration-500">
					<i :data-feather="social.icon" class="w-5 h-5"></i>
				</a>
			</ul>
		</div>


		<div class="font-general-regular text-lg text-gray">
			&copy; {{ copyrightDate }} {{ projectName }}

			<!-- <a
				href="https://github.com/realstoman/vuejs-tailwindcss-portfolio"
				target="__blank"
				class="font-general-medium hover:underline hover:text-indigo-600 dark:hover:text-indigo-300 duration-500"
			>
			{{ projectName }}
			</a> -->
			<!-- . Developed by
			<a
				href="https://stoman.me"
				target="__blank"
				class="font-general-medium text-secondary-dark dark:text-secondary-light uppercase hover:underline hover:text-indigo-600 dark:hover:text-indigo-300 duration-500"
				>{{ author }}</a
			> -->

		</div>
	</div>
</template>

<style lang="scss" scoped>
</style>
