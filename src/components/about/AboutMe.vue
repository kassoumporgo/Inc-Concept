<script>
export default {
	setup() {
		return {
			bios: [
			
				{
					id: 1,
					bio:
						'Incorporated Concept (Inc Concept) est une agence de prestation de services située à Ouagadougou, capitale politique du Burkina Faso. L’agence est animée par des équipes jeunes, dynamiques et compétentes dans un esprit d’innovation. Nous proposons des Solutions Complètes, Innovantes et Intégrées en prestation de services dans le domaine de la Formation-Appui-Conseil, de la Communication, du Recrutement-placement et de la Gestion d’affaires et la Distribution.',
				},

				{
					id: 2,
					bio:
						'Nous aspirons apporter à nos clients et à nos partenaires un appui technique adéquat et professionnel. Nous nous donnons pour mission d’offrir des services sur mesure et adaptés à chaque secteur d’activité, avec les besoins variés. En somme, il s’agit pour Inc Concept de proposer des actions ciblées et adaptées à chaque réalité clientèle ; conceptualiser chaque besoin !',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<!-- <div class="w-full sm:w-1/4 mb-7 sm:mb-0">

			<img
				src="@/assets/images/profile.jpeg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div> -->

		<!-- About details -->
		<!-- <div class="w-full sm:w-3/4 text-left"> -->

	


		<div class="w-full text-left">

			<div class="font-general-semibold text-3xl sm:text-4xl font-semibold text-primary-dark dark:text-primary-light mb-8">
				<h4>Qui somme nous ?</h4>
			</div>

			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
