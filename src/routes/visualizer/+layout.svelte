<script>
	import { AppShell, AppRail, AppRailAnchor } from '@skeletonlabs/skeleton';
	import { page } from '$app/stores';
</script>

<body>
	<AppShell>
		<svelte:fragment slot="sidebarLeft">
			<AppRail>
				<AppRailAnchor
					href="/visualizer/initialize"
					selected={$page.url.pathname === '/visualizer/initialize'}>Initialize</AppRailAnchor
				>
				<AppRailAnchor
					href="/visualizer/activations"
					selected={$page.url.pathname === '/visualizer/activations'}>Activations</AppRailAnchor
				>
				<AppRailAnchor
					href="/visualizer/weights"
					selected={$page.url.pathname === '/visualizer/weights'}>Weights</AppRailAnchor
				>
				<AppRailAnchor
					href="/visualizer/metrics"
					selected={$page.url.pathname === '/visualizer/metrics'}>Metrics</AppRailAnchor
				>
			</AppRail>
		</svelte:fragment>
		<slot />
	</AppShell>
</body>
