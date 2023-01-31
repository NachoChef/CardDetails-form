<script lang="ts">
	import bgMainDesktop from '$lib/assets/bg-main-desktop.png';
	import bgCardFront from '$lib/assets/bg-card-front.png';
	import bgCardBack from '$lib/assets/bg-card-back.png';
	import CcForm from '$lib/components/CCForm.svelte';
</script>

<img src={bgMainDesktop} alt="side logo" srcset="" />
<div class="card-front">
	<img src={bgCardFront} alt="" class="card-front" />
	<img src={bgCardBack} alt="" class="card-back" />
</div>

<CcForm />

<style>
	/* def need a media query but will start with desktop */
</style>
