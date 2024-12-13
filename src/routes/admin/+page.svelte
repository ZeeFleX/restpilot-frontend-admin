<script lang="ts">
	import { Breadcrumbs } from '$lib/components/admin/breadcrumbs';
	import { DollarSign, Users } from 'lucide-svelte';
	import { Summary } from '$lib/components/admin/widgets';
</script>

<div class="flex flex-col gap-6">
	<Breadcrumbs />
	<div class="grid gap-4 md:grid-cols-2 md:gap-8 lg:grid-cols-4">
		<Summary
			title="Заказов за неделю на сумму"
			value={14500}
			scale={'+6%'}
			scaleText="По сравнению с прошлой неделей"
			icon={DollarSign}
		/>
		<Summary
			title="Заказов за месяц на суму"
			value={64800}
			scale={'+12.5%'}
			scaleText="По сравнению с прошлым месяцем"
			icon={DollarSign}
		/>
		<Summary
			title="Новых пользователей за месяц"
			value={158}
			scale={'+4%'}
			scaleText="По сравнению с прошлым месяцем"
			icon={Users}
		/>
	</div>
</div>

<style lang="postcss"></style>
