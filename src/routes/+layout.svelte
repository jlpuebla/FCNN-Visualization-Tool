<script lang="ts">
	import '../app.postcss';

	// Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
	import { storePopup } from '@skeletonlabs/skeleton';
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });


	import { AppShell, AppBar } from '@skeletonlabs/skeleton';
</script>

<body>
	<AppShell>
		<svelte:fragment slot="header">
			<AppBar>
				<!--Logo will go here later-->
				Fully-Connected Feed-Forward Neural Network Visualizer
			</AppBar>

			<AppBar
				gridColumns="grid-cols-3"
				slotDefault="place-self-center"
				slotTrail="place-content-end"
			>
				<svelte:fragment slot="lead">
					<a href="/">Home</a>
					<a href="/create">Create</a>
					<a href="/definitions">Definitions</a>
				</svelte:fragment>
			</AppBar>
		</svelte:fragment>
		<!-- (sidebarLeft) -->
		<!-- (sidebarRight) -->
		<!-- (pageHeader) -->
		<!-- Router Slot -->
		<slot />
		<!-- ---- / ---- -->
		<svelte:fragment slot="pageFooter">CR2G Lab</svelte:fragment>
		<!-- (footer) -->
	</AppShell>
</body>


<slot />
