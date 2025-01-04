<script lang="ts">
	import '../app.css';
	import { AppBar, AppShell } from '@skeletonlabs/skeleton';
	let { children } = $props();
</script>

<AppShell slotSidebarLeft="bg-surface-500/5 w-56 p-4">
	<svelte:fragment slot="sidebarLeft">
		<!-- Insert the list: -->
		<nav class="list-nav">
			<ul>
				<li><a href="/">Home</a></li>
				<!-- <li><a href="/about">About</a></li> -->
			</ul>
		</nav>
		<!-- --- -->
	</svelte:fragment>
	{@render children()}
	<svelte:fragment slot="header">
		<AppBar>Skeleton</AppBar>
	</svelte:fragment>
</AppShell>
