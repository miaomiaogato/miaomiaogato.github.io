<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { base } from '$app/paths';

	let { children } = $props();

	const navItems = [
		{ path: '/', label: 'home' },
		{ path: '/about', label: 'about me' },
		{ path: '/blog', label: 'blog' },
		{ path: '/contact', label: 'contact me' }
	];
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="layout-container min-h-screen">
	<div class="flex justify-center items-center min-h-screen py-8 relative">
		<aside class="sidebar absolute flex flex-col items-start px-6 py-8">
			<nav class="flex flex-col gap-4">
				{#each navItems as item}
					<a href={base + item.path} class="nav-link text-lg lowercase">
						{item.label}
					</a>
				{/each}
			</nav>
		</aside>

		<main class="w-[800px] h-[800px] px-8 py-8 overflow-auto">
			{@render children()}
		</main>
	</div>
</div>
