<script lang="ts">
	// something
	export let name: string = '';
	export let expiryMonth: string = '';
	export let expiryYear: string = '';
	export let cardNumber: string = '';
	export let cvc: string = '';
</script>

<form action="submit" class="cc-form" style="--width:400px">
	<label>
		Cardholder Name
		<input type="text" placeholder="e.g. Jane Appleseed" bind:value={name} />
	</label>
	<label>
		Card Number
		<input
			type="text"
			inputmode="numeric"
			pattern="[0-9]+"
			placeholder="e.g. 1234 5678 9123 000"
			bind:value={cardNumber}
			maxlength="16"
		/>
	</label>
	<label>
		Exp. Date (MM/YY)
		<input
			type="text"
			inputmode="numeric"
			pattern="[0-9]+"
			placeholder="MM"
			bind:value={expiryMonth}
			maxlength="2"
		/>
		<input
			type="text"
			inputmode="numeric"
			pattern="[0-9]+"
			placeholder="YY"
			bind:value={expiryYear}
			maxlength="2"
		/>
	</label>
	<label>
		CVC
		<input
			type="text"
			inputmode="numeric"
			pattern="[0-9]+"
			placeholder="e.g. 123"
			bind:value={cvc}
			maxlength="3"
		/>
	</label>
	<button class="btn">Confirm</button>
</form>

<style>
	.cc-form {
		width: var(--width);
	}

	.btn {
		width: var(--width);
		height: 40px;
		border: none;
		display: flex;
		justify-content: center;
		align-items: center;
		border-radius: 5px;
		color: var(--white);
		background-color: var(--very-dark-violet);
	}

	input {
		border-radius: 5px;
		height: 40px;
		font-size: 1em;
		border-style: 1px solid var(--dark-grayish-violet);
	}

	label {
		display: flex;
		flex-direction: column;
		color: var(--very-dark-violet);
	}
</style>
