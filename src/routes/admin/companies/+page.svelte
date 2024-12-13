<script lang="ts">
	import { Breadcrumbs } from '$lib/components/admin/breadcrumbs';
	import * as Card from '$lib/components/ui/card/index.js';
	import { CompaniesTable } from '$lib/components/admin/tables';
	import { companies } from './constants';
</script>

<div class="flex flex-col gap-6">
	<Breadcrumbs />
	<Card.Root>
		<Card.Header>
			<Card.Title>Компании</Card.Title>
		</Card.Header>
		<Card.Content>
			<CompaniesTable {companies} />
		</Card.Content>
	</Card.Root>
</div>

<style lang="postcss">
</style>
