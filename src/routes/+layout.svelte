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
				<li><a href="/">Experiences</a></li>
				<li><a href="/cert">Certificate & Achievement</a></li>
				<li><a href="/iot">My IoT Stuff</a></li>
				<li><a href="/laptops">My Laptops</a></li>
				<li><a href="/keyboards">My Mechanical Keyboards</a></li>
				<li><a href="/links">Link</a></li>
			</ul>
		</nav>
		<!-- --- -->
	</svelte:fragment>
	{@render children()}
	<svelte:fragment slot="header">
		<AppBar>Tran Viet Anh</AppBar>
	</svelte:fragment>
</AppShell>
