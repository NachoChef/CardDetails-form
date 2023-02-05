<script lang="ts">
	import bgCardBack from '$lib/assets/bg-card-back.png';

	export let cvc: string;
</script>

<div class="card-back" style="--imgUrl:url({bgCardBack});">
	<span class="cvc">
		{cvc}
	</span>
</div>

<style>
	.card-back {
		background-image: var(--imgUrl);
		background-repeat: no-repeat;
		height: 250px;
		width: 450px;
		position: relative;
	}

	.cvc {
		position: absolute;
		top: 110px;
		right: 55px;
		letter-spacing: 1px;
		color: var(--white);
	}
</style>
