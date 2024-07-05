<script lang="ts">
	import { onMount } from 'svelte';
	import { createNeuralNetwork } from '$lib/neuralNetwork';

	
	onMount( () =>{
		document.getElementById('btn_train_test')?.addEventListener('click', createNeuralNetwork )
	})

	

</script>

<div class="rounded-xl p-8">
	<span class="h2">Initialize Fully-Connected Neural Network</span>

	<label class="label">
		<span>Network</span>
		<select class="select">
			<option value="custom">Custom Network</option>
			<option value="network1">Network 1</option>
			<option value="network2">Network 2</option>
		</select>
	</label>

	<label class="label">
		<span>Dataset</span>
		<select class="select">
			<option value="mnist">MNIST</option>
			<option value="other">Other</option>
		</select>
	</label>

	<span class="h3">Hidden Layers:</span>

	<label class="label">
		<span>Layers</span>
		<input class="input" type="text" placeholder="0" />
	</label>

	<label class="label">
		<span>Nodes</span>
		<input class="input" type="text" placeholder="0" />
	</label>

	<label class="label">
		<span>Activation Function</span>
		<select class="select">
			<option value="relu">ReLU</option>
			<option value="leakyRely">Leaky ReLU</option>
			<option value="tanH">tanH</option>
			<option value="softmax">softmax</option>
		</select>
	</label>

	<span class="h3">Output Layer:</span>

	<label class="label">
		<span>Nodes</span>
		<input class="input" type="text" placeholder="0" />
	</label>

	<label class="label">
		<span>Activation Function</span>
		<select class="select">
			<option value="relu">ReLU</option>
			<option value="leakyRely">Leaky ReLU</option>
			<option value="tanH">tanH</option>
			<option value="softmax">softmax</option>
		</select>
	</label>

	<a href="#" class="btn variant-filled-surface" id="btn_train_test">Train & Test</a>
</div>