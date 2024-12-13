<script lang="ts">
	import { Sidebar } from '$lib/components/admin';
	let { children } = $props();
</script>

<div class="bg-muted/40 flex min-h-screen w-full flex-col">
	<Sidebar />
	<div class="flex-1 pl-20 pr-6 pt-4">
		{@render children()}
	</div>
</div>

<style lang="postcss"></style>
