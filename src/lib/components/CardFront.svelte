<script lang="ts">
	import bgCardFront from '$lib/assets/bg-card-front.png';

	let name: string = 'Jane Doe';
	let expiryMonth: string = '00';
	let expiryYear: string = '00';
	let cardNumber: string = '0000 0000 0000 0000';
</script>

<div class="card-front" style="--imgUrl:url({bgCardFront});">
	<span class="card-number">
		{cardNumber}
	</span>
	<span class="name">
		{name}
	</span>
	<span class="date">
		{expiryMonth}/{expiryYear}
	</span>
</div>

<style>
	.card-front {
		background-image: var(--imgUrl);
		background-repeat: no-repeat;
		height: 250px;
		width: 450px;
		position: relative;
	}

	.card-number {
		font-size: 30px;
		font-family: 'Comic Sans MS';
		position: absolute;
		top: 140px;
		letter-spacing: 4px;
		text-align: center;
		color: white;
		width: 100%;
	}

	.name {
		font-size: 16px;
		font-family: 'Open Sans', sans-serif;
		position: absolute;
		top: 200px;
		left: 30px;
		letter-spacing: 2px;
		color: white;
	}

	.date {
		font-size: 16px;
		font-family: 'Open Sans', sans-serif;
		position: absolute;
		top: 200px;
		right: 30px;
		letter-spacing: 2px;
		color: white;
	}
</style>
