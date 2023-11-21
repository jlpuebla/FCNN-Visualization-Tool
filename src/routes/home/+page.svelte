<script lang="ts">
	import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
</script>

<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-10 text-justify flex flex-col items-center">
		<strong class="text-lg italic">
			<h1 class="h2">How Does a Neural Network Work?</h1>
		</strong>
		<div class="transition-colors">
			<Accordion autocollapse>
				<AccordionItem open>
					<svelte:fragment slot="summary">
						<h2 class="h2">Parts</h2>
					</svelte:fragment>
					<svelte:fragment slot="content">
						<h4 class="h4">Nodes</h4>
						<p class="p-4">
							Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab accusamus odit quis,
							voluptatum iusto doloremque adipisci facere vel amet non a facilis corrupti nihil
							expedita reprehenderit quod ducimus tempora numquam!
						</p>
						<h4 class="h4">Weights</h4>
						<p class="p-4">
							Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque illum, quibusdam quam
							distinctio, quas pariatur odio odit repellat quia aspernatur vel saepe. Corrupti
							deleniti natus voluptatem necessitatibus magni, iusto fugit.
						</p>
						<h4 class="h4">Layers</h4>
						<p class="p-4">
							Lorem ipsum dolor sit amet consectetur adipisicing elit. Atque illum, quibusdam quam
							distinctio, quas pariatur odio odit repellat quia aspernatur vel saepe. Corrupti
							deleniti natus voluptatem necessitatibus magni, iusto fugit.
						</p>
					</svelte:fragment>
				</AccordionItem>
				<AccordionItem>
					<svelte:fragment slot="summary">
						<h2 class="h2">Training</h2>
					</svelte:fragment>
					<svelte:fragment slot="content">
						<p class="p-4">
							Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore
							culpa sint ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim
							cupidatat excepteur officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip
							amet voluptate voluptate dolor minim nulla est proident. Nostrud officia pariatur ut
							officia. Sit irure elit esse ea nulla sunt ex occaecat reprehenderit commodo officia
							dolor Lorem duis laboris cupidatat officia voluptate. Culpa proident adipisicing id
							nulla nisi laboris ex in Lorem sunt duis officia eiusmod. Aliqua reprehenderit commodo
							ex non excepteur duis sunt velit enim. Voluptate laboris sint cupidatat ullamco ut ea
							consectetur et est culpa et culpa duis.
						</p>
					</svelte:fragment>
				</AccordionItem>
				<AccordionItem>
					<svelte:fragment slot="summary">
						<h2 class="h2">Optimizing</h2>
					</svelte:fragment>
					<svelte:fragment slot="content">
						<p class="4">
							Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum nam inventore assumenda
							ratione tempore aut omnis, nisi id dolores dolorem, incidunt praesentium amet impedit.
							Veniam facere dolorum nihil officia eos.
						</p>
					</svelte:fragment>
				</AccordionItem>
				<AccordionItem>
					<svelte:fragment slot="summary">
						<h2 class="h2">Challenges</h2>
					</svelte:fragment>
					<svelte:fragment slot="content">
						<p class="p-4">
							Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore
							culpa sint ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim
							cupidatat excepteur officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip
							amet voluptate voluptate dolor minim nulla est proident. Nostrud officia pariatur ut
							officia. Sit irure elit esse ea nulla sunt ex occaecat reprehenderit commodo officia
							dolor Lorem duis laboris cupidatat officia voluptate. Culpa proident adipisicing id
							nulla nisi laboris ex in Lorem sunt duis officia eiusmod. Aliqua reprehenderit commodo
							ex non excepteur duis sunt velit enim. Voluptate laboris sint cupidatat ullamco ut ea
							consectetur et est culpa et culpa duis.
						</p>
					</svelte:fragment>
				</AccordionItem>
			</Accordion>
		</div>
	</div>
</div>
