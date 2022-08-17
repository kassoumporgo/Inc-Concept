<script>
// import ThemeSwitcher from '../ThemeSwitcher';
// import HireMeModal from '../HireMeModal.vue';
import feather from 'feather-icons';
import AppHeaderLinks from './AppHeaderLinks.vue';
import Button from '../reusable/Button.vue';

export default {
	components: {
		// ThemeSwitcher,
		// HireMeModal,
		AppHeaderLinks,
		Button,
	},
	data() {
		return {
			isOpen: false,
			theme: '',
			modal: false,
		};
	},

	created() {
		this.theme = localStorage.getItem('theme') || 'light';
	},
	mounted() {
		feather.replace();
		this.theme = localStorage.getItem('theme') || 'light';
	},
	methods: {
		updateTheme(theme) {
			this.theme = theme;
		},
		showModal() {
			if (this.modal) {
				document
					.getElementsByTagName('html')[0]
					.classList.remove('overflow-y-hidden');
				this.modal = false;
			} else {
				document
					.getElementsByTagName('html')[0]
					.classList.add('overflow-y-hidden');
				this.modal = true;
			}
		},
	},
	updated() {
		feather.replace();
	},
};
</script>



<template>
	<nav id="nav" class="sm:pl-0 md:pl-5 block sticky top-0 bg-main0">

		<div class="z-10 max-w-screen-lg xl:max-w-screen-xl block sm:flex sm:justify-between sm:items-center my-0">

			<div class="flex justify-between items-center px-4 sm:px-0">

				<div>
					<router-link to="/"><img src="@/assets/images/logo-vect.png" class="w-26 h-16" alt="Logo" />
					</router-link>
				</div>



				<!-- <theme-switcher :theme="theme" @themeChanged="updateTheme"
					class="block sm:hidden bg-ternary-light dark:bg-ternary-dark hover:bg-hover-light dark:hover:bg-hover-dark hover:shadow-sm px-2.5 py-2 rounded-lg" /> -->

				<!-- Hamburger menu (Smartphone) -->
				<div class="sm:hidden">
					<button @click="isOpen = !isOpen" type="button" class="focus:outline-none"
						aria-label="Hamburger Menu">
						<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
							class="h-7 w-7 fill-current text-secondary-dark dark:text-ternary-light">
							<path v-if="isOpen" fill-rule="evenodd"
								d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"
								clip-rule="evenodd"></path>
							<path v-if="!isOpen" fill-rule="evenodd"
								d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z">
							</path>
						</svg>
					</button>
				</div>
			</div>

			<AppHeaderLinks :showModal="showModal" :isOpen="isOpen" />

			<div class="hidden sm:flex justify-between items-center flex-col md:flex-row">

				<router-link to="/contact"
					class="text-md font-general-medium bg-indigo-500 text-white shadow-sm rounded-full px-5 py-2.5"
					aria-label="">
					<Button class="text-white" title="Nous contacter" />
				</router-link>

				<!-- <theme-switcher :theme="theme" @themeChanged="updateTheme"
					class="ml-8 bg-primary-light dark:bg-ternary-dark px-3 py-2 shadow-sm rounded-full cursor-pointer" /> -->

			</div>


		</div>

		<!-- Hire me modal -->
		<!-- <HireMeModal
			:showModal="showModal"
			:modal="modal"
			:categories="categories"
			aria-modal="Hire Me Modal"
		/> -->
	</nav>
</template>



<style scoped>
/* #nav a.router-link-exact-active {
	@apply text-indigo-700;
	@apply dark: text-indigo-400;
	@apply font-medium;
} */
</style>
