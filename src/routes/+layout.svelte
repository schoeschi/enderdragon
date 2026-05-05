<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { ModeWatcher } from 'mode-watcher';
	import { LightRays } from '$lib/components/magic/light-rays';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<ModeWatcher />
<main class="flex h-screen flex-col items-center justify-center gap-6 text-center">
	<LightRays />
	{@render children()}
</main>
