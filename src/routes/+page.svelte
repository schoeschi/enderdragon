<script lang="ts">
	import { Button } from '$lib/components/ui/button';
	import { Badge } from '$lib/components/ui/badge';
	import { Users } from '@lucide/svelte';
	import * as Card from '$lib/components/ui/card/index.js';
</script>

<Badge
	variant="outline"
	class="border-primary/50 bg-primary/10 text-primary dark:border-white/50 dark:bg-white/30 dark:text-white"
>
	<Users /> 2 players online
</Badge>

<h1 class="max-w-4xl text-5xl font-black tracking-tighter sm:text-7xl lg:text-8xl">
	Join <span class="text-primary">Enderdragon</span>.
</h1>

<Card.Root class="p-2 shadow-xl">
	<Card.Content class="flex items-center gap-2 p-0 pl-2">
		<code class="font-mono font-bold text-primary dark:text-white">mc.enderdragon.ch</code>
		<Button size="sm">Copy IP</Button>
	</Card.Content>
</Card.Root>
