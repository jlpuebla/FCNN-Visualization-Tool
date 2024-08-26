<script lang="ts">
	import { createNeuralNetwork } from '$lib/neuralNetwork';

	// https://svelte.dev/repl/74685aa8b4374c4c8f395ce643fee7b6?version=3.48.0
	const onSubmit = (e:any) => {
		const ACTION_URL = e.target.action

		const formData = new FormData(e.target);
		const data = new URLSearchParams();

		for (let field of formData) {
			const [key, value] = field;
			data.append(key, value);
		}
		createNeuralNetwork(data.get('hiddenLayers'), data.get('hiddenNodes'), data.get('hiddenActivationFunction'),
		data.get('outputNodes'), data.get('outputActivationFunction'))
	}

</script>

<div class="rounded-xl p-8">
	<span class="h2">Initialize Fully-Connected Neural Network</span>

	<form on:submit|preventDefault={onSubmit}>
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
			<input id="formHiddenLayers" class="input" type="text" name="hiddenLayers" placeholder="0" value=""/>
		</label>

		<label class="label">
			<span>Nodes</span>
			<input id="formHiddenNodes" class="input" type="text" name="hiddenNodes" placeholder="0" />
		</label>

		<label class="label">
			<span>Activation Function</span>
			<select id="formHiddenActivationFunction" name="hiddenActivationFunction" class="select">
				<option value="relu">ReLU</option>
				<option value="leakyRely">Leaky ReLU</option>
				<option value="tanH">tanH</option>
				<option value="softmax">softmax</option>
			</select>
		</label>

		<span class="h3">Output Layer:</span>

		<label class="label">
			<span>Nodes</span>
			<input id="formOutputNodes" class="input" type="text" name="outputNodes" placeholder="0" />
		</label>

		<label class="label">
			<span>Activation Function</span>
			<select id="formOutputActivationFunction" name="outputActivationFunction" class="select">
				<option value="relu">ReLU</option>
				<option value="leakyRely">Leaky ReLU</option>
				<option value="tanH">tanH</option>
				<option value="softmax">softmax</option>
			</select>
		</label>
		
		<input type="submit" value="Train & Test">
	</form>
</div>
