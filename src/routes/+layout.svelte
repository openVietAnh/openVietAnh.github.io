<script lang="ts">
	import '../app.css';
	import { AppBar, AppShell } from '@skeletonlabs/skeleton';
	let { children } = $props();
</script>

<AppShell slotSidebarLeft="bg-surface-500/5 w-56 p-4">
	<svelte:fragment slot="sidebarLeft">
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
	</svelte:fragment>
	{@render children()}
	<svelte:fragment slot="header">
		<AppBar class="!bg-[#f2e5bc] border-b-2 border-[#928374]"><h5>Tran Viet Anh - (+84) 988 582 914 - vietanhtran.uet@gmail.com</h5></AppBar>
	</svelte:fragment>
</AppShell>
