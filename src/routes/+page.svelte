<script lang="ts">
	import bgMainDesktop from '$lib/assets/bg-main-desktop.png';
	import bgCardBack from '$lib/assets/bg-card-back.png';
	import CcForm from '$lib/components/CCForm.svelte';
	import CardFront from '$lib/components/CardFront.svelte';
	import '@fontsource/space-grotesk';
	import CardBack from '$lib/components/CardBack.svelte';

	let name: string = '';
	let expiryMonth: string;
	let expiryYear: string;
	let cardNumber: string;
	let cvc: string;
</script>

<!-- <img src={bgMainDesktop} alt="side logo" srcset="" /> -->
<div class="card">
	<CardFront {name} {expiryMonth} {expiryYear} {cardNumber} />
	<CardBack cvc="123" />
</div>

<CcForm bind:name bind:expiryMonth bind:expiryYear bind:cardNumber />

<style>
	/* def need a media query but will start with desktop */
	:global(:root) {
		--white: hsl(0, 0%, 100%);
		--light-grayish-violet: hsl(270, 3%, 87%);
		--dark-grayish-violet: hsl(279, 6%, 55%);
		--very-dark-violet: hsl(278, 68%, 11%);
		font-family: 'Space Grotesk';
	}
</style>
