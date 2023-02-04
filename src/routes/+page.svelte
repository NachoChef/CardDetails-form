<script lang="ts">
	import bgMainDesktop from '$lib/assets/bg-main-desktop.png';
	import bgCardBack from '$lib/assets/bg-card-back.png';
	import CcForm from '$lib/components/CCForm.svelte';
	import CardFront from '$lib/components/CardFront.svelte';

	let name: string;
	let expiryMonth: string;
	let expiryYear: string;
	let cardNumber: string;
</script>

<!-- <img src={bgMainDesktop} alt="side logo" srcset="" /> -->
<div class="card">
	<CardFront {name} {expiryMonth} {expiryYear} {cardNumber} />
	<!-- <img src={bgCardBack} alt="" class="card-back" /> -->
</div>

<CcForm bind:name bind:expiryMonth bind:expiryYear bind:cardNumber />

<style>
	/* def need a media query but will start with desktop */
</style>
