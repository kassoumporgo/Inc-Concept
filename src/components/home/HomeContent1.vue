
<script>
export default {
	setup() {
		return {

			ourBio: "Destine aux entreprise, association, ddudud ddid dddi ddod ddod dood dkd vnv fkkkd dkskd dkdk",

			aboutUsDes: [
				{
					id: 1,
					title: 'Pole consulting',
					des: 'hdjhdhd dkdkkd dkdkkd dkdkd dkdkd dkdkd l.'
				},
				{
					id: 2,
					title: 'Pole design & comminunication',
					des: 'hdjhdhd dkdkkd dkdkkd dkdkd dkdkd dkdkd l.'
				},
				{
					id: 3,
					title: 'Pole evenementiel',
					des: 'hdjhdhd dkdkkd dkdkkd dkdkd dkdkd dkdkd l.'
				},
			],
		};
	},
};
</script>


<template>

	<div class="container mx-auto flex flex-col-reverse md:flex-row py-5">

		<div class="w-full md:w-1/2 md:pr-5">

			<div class="flex flex-col text-left mb-2">

				<p class="font-general-semibold text-2xl font-semibold text-primary-dark dark:text-primary-light mb-5">
					POURQUOI Inc Concept ?
				</p>

				<div class="">
					<p>{{ ourBio }}</p>
				</div>



				<div v-for="item in aboutUsDes" :key="item.id" target="__blank" class="pt-3 pl-5">

					<span class="font-bold uppercase">{{ item.title }}</span>
					<p>{{ item.des }}</p>

				</div>


			</div>

		</div>

		<div class="w-full md:w-1/2 md:pl-5">

			<div class="flex flex-col text-left mb-2 md:ml-10">
				<p class="font-general-semibold text-2xl font-semibold text-primary-dark dark:text-primary-light mb-5">
					ACTUALITE
				</p>

				<div class="">

					<img src="@/assets/images/web-project-1.jpg" alt="" class="h-60">


				</div>

			</div>

		</div>

	</div>

</template>