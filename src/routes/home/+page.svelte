<script lang="ts">
	import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';

  let parts = 'Parts';
  let parts_about = 
    'A neural network is meant to represent a rudimentary version of the brain, ' +
    'which is further highlighted by some of the terminology, with a single purpose of ' +
    'helping the computer make intelligent decisions withlimited human assistance. ' +
    'These decisions include a vast range, such as image classification, sentiment analysis, ' +
    'and signal processing, to name a few.<br><br>Following is some terminology ' +
    'along with their definitions:<br><br>';
  let parts_nodes = 'Nodes';
  let nodes_about =  'Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat.<br>';
  let parts_weights = 'Weights';
  let weights_about = 'Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat.<br>';
  let parts_layers = 'Layers';
  let layers_about = 'Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat.<br>';
  let parts_biases = 'Bias'
  let biases_about = 'Lorem ipsum dolor sit amet, qui minim labore adipisicing minim sint cillum sint consectetur cupidatat.<br>';

  let training = 'Training';
  let optimizing = 'Optimizing';
  let challenges = 'Challenges';
</script>

<div class="container h-full mx-auto flex justify-center items-center p-28">
	<div class="space-y-10 text-justify flex flex-col items-center">
		<strong class="text-lg italic">
			<h1 class="h2">How Does a Neural Network Work?</h1>
		</strong>
		<div class="transition-colors">
			<Accordion autocollapse>
				<AccordionItem open>
					<svelte:fragment slot="summary">
						<strong><h3 class="h3">{parts}</h3></strong>
					</svelte:fragment>
					<svelte:fragment slot="content">
            <div class="p-4">
              <p class="p-4">
                {@html parts_about}
              </p>
						  <h3 class="h3">{parts_nodes}</h3>
						  <p class="p-4">
                {@html nodes_about}
						  </p>
						  <h3 class="h3">{parts_weights}</h3>
						  <p class="p-4">
                {weights_about}
						  </p>
						  <h3 class="h3">{parts_layers}</h3>
						  <p class="p-4">
                {layers_about}
						  </p>
              <h3 class="h3">{parts_biases}</h3>
              <p class="p-4">
                {biases_about}
              </p>
            </div>
					</svelte:fragment>
				</AccordionItem>
				<AccordionItem>
					<svelte:fragment slot="summary">
						<strong><h3 class="h3">{training}</h3></strong>
					</svelte:fragment>
					<svelte:fragment slot="content">
            <div class="p-4">
              <p class="p-4">
                Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.

              </p>
            </div>
					</svelte:fragment>
				</AccordionItem>
				<AccordionItem>
					<svelte:fragment slot="summary">
						<strong><h3 class="h3">{optimizing}</h3></strong>
					</svelte:fragment>
					<svelte:fragment slot="content">
            <div class="p-4">
					  	<p class="4">
					  		Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum nam inventore assumenda
					  		ratione tempore aut omnis, nisi id dolores dolorem, incidunt praesentium amet impedit.
					  		Veniam facere dolorum nihil officia eos.
					  	</p>
            </div>
					</svelte:fragment>
				</AccordionItem>
				<AccordionItem>
					<svelte:fragment slot="summary">
						<strong><h3 class="h3">{challenges}</h3></strong>
					</svelte:fragment>
					<svelte:fragment slot="content">
            <div class="p-4">
              <p class="p-4">
                Lorem ipsum dolor sit amet, officia excepteur ex fugiat reprehenderit enim labore culpa sint ad nisi Lorem pariatur mollit ex esse exercitation amet. Nisi anim cupidatat excepteur officia. Reprehenderit nostrud nostrud ipsum Lorem est aliquip amet voluptate voluptate dolor minim nulla est proident. Nostrud officia pariatur ut officia. Sit irure elit esse ea nulla sunt ex occaecat reprehenderit commodo officia dolor Lorem duis laboris cupidatat officia voluptate. Culpa proident adipisicing id nulla nisi laboris ex in Lorem sunt duis officia eiusmod. Aliqua reprehenderit commodo ex non excepteur duis sunt velit enim. Voluptate laboris sint cupidatat ullamco ut ea consectetur et est culpa et culpa duis.
              </p>
            </div>
					</svelte:fragment>
				</AccordionItem>
			</Accordion>
		</div>
	</div>
</div>
