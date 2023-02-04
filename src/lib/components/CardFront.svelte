<script lang="ts">
	import bgCardFront from '$lib/assets/bg-card-front.png';

	export let userName: string = 'Jane Doe';
	export let expiryMonth: string = '00';
	export let expiryYear: string = '00';
	export let cardNumber: string = '0000000000000000';
</script>

<div class="card-front">
	<span class="card-number">
		{cardNumber}
	</span>
</div>

<style>
	.card-front {
		background-image: bgCardFront;
	}
</style>
