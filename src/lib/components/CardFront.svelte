<script lang="ts">
	import bgCardFront from '$lib/assets/bg-card-front.png';
	import cardLogo from '$lib/assets/card-logo.svg';

	export let name: string = 'Jane Doe';
	let expiryMonth: string = '00';
	let expiryYear: string = '00';
	let cardNumber: string = '0000 0000 0000 0000';
</script>

<div class="card-front" style="--imgUrl:url({bgCardFront});">
	<span class="logo">
		<img src={cardLogo} alt="logo" />
	</span>
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
		position: absolute;
		top: 140px;
		letter-spacing: 4px;
		text-align: center;
		color: var(--white);
		width: 100%;
	}

	.date {
		font-size: 16px;
		position: absolute;
		top: 200px;
		right: 25px;
		letter-spacing: 2px;
		color: var(--white);
	}

	.name {
		font-size: 16px;
		position: absolute;
		top: 200px;
		left: 25px;
		letter-spacing: 2px;
		color: var(--white);
	}

	.logo {
		position: absolute;
		top: 30px;
		left: 25px;
	}
</style>
