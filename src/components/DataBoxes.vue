<template>
	<div class="grid gap-4 md:grid-cols-2">
		<div class="p-10 text-center bg-green-400 rounded shadow-md">
			<h3 class="mb-4 text-3xl font-bold text-blue-900">Cases</h3>
			<div class="mb-4 text-2xl">
				<span class="font-bold">New:</span>
				{{ stats.NewConfirmed }}
			</div>
			<div class="mb-4 text-2xl">
				<span class="font-bold">Total:</span>
				{{ stats.TotalConfirmed }}
			</div>
		</div>

		<div class="p-10 text-center bg-green-400 rounded shadow-md">
			<h3 class="mb-4 text-3xl font-bold text-blue-900">Deaths</h3>
			<div class="mb-4 text-2xl">
				<span class="font-bold">New:</span>
				{{ stats.NewDeaths }}
			</div>
			<div class="mb-4 text-2xl">
				<span class="font-bold">Total:</span>
				{{ stats.TotalDeaths }}
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: "DataBoxes",
		props: ["stats"]
	};
</script>
