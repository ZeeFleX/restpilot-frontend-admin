<script lang="ts">
	import { Breadcrumbs } from '$lib/components/admin/breadcrumbs';
	let { children } = $props();
</script>

<div class="flex flex-col gap-6">
	<Breadcrumbs />
	{@render children()}
</div>

<style lang="postcss"></style>
