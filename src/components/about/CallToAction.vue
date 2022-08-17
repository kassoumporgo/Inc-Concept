<!-- <script>
import counter from 'vue3-autocounter';
export default {
	components: {
		counter,
	},
	data: () => {
		return {
			experienceTitle: "Années d'experience",
			feedbackTitle: 'Avis positifs',
			projectsTitle: 'Projets réalisés',
		};
	},
};
</script> -->


<template>
	<div class="bg-primary-light dark:bg-ternary-dark shadow-sm">
	
		<div
			class="font-general-regular container mx-auto py-10 block sm:flex sm:justify-between sm:items-center"
		>

        <div class="center">
            <h1>Comme eux, confiez-nous la realisation de votre projet digital.</h1>
        </div>
			
			<!-- <div class="mb-10 sm:mb-0">
				<counter
					ref="counter"
					:startAmount="0"
					:endAmount="12"
					:duration="1"
					:autoinit="true"
					@finished="alert(`Counting finished!`)"
					class="font-general-medium text-5xl font-bold text-main0 dark:text-main0 mb-2"
					aria-label="About Status Counter"
				/>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light mt-5"
				>
					{{ experienceTitle }}
				</span>
			</div>

	
			<div class="mb-10 sm:mb-0">
				<counter
					ref="counter"
					:startAmount="0"
					:endAmount="92"
					:duration="1"
					suffix="%"
					:autoinit="true"
					@finished="alert(`Counting finished!`)"
					class="font-general-medium text-5xl font-bold text-main0 dark:text-main0 mb-2"
				/>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light mt-5"
				>
					{{ feedbackTitle }}
				</span>
			</div>

			
			<div class="mb-10 sm:mb-0">
				<counter
					ref="counter"
					:startAmount="0"
					:endAmount="77"
					:duration="1"
					:autoinit="true"
					@finished="alert(`Counting finished!`)"
					class="font-general-medium text-5xl font-bold text-main0 dark:text-main0 mb-2"
				/>
				<span
					class="block text-md text-ternary-dark dark:text-ternary-light mt-5"
				>
					{{ projectsTitle }}
				</span>
			</div> -->

		</div>
	</div>
</template>
