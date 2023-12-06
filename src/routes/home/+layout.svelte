<script lang="ts">
	import { AppShell, AppBar } from '@skeletonlabs/skeleton';
	import { goto } from '$app/navigation';
</script>

<body>
	<AppShell>
		<svelte:fragment slot="header">
			<AppBar
				gridColumns="grid-cols-3"
				slotDefault="place-self-center"
				slotTrail="place-content-end"
			>
				<svelte:fragment slot="lead">
					<button on:click={() => goto('home')}>
						<strong class="text-xl font-bold">
							Fully Connected Neural Network Visualization Tool
						</strong>
					</button>
				</svelte:fragment>
				<svelte:fragment slot="trail">
					<button
						type="button"
						class="btn-icon btn-icon-lg variant-filled"
						on:click={() => goto('main')}
					>
						main
					</button>
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
