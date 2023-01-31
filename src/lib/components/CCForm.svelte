<script>
	// something
</script>

<form action="submit" class="cc-form" style="--width:400px">
	<label>
		Cardholder Name
		<input type="text" placeholder="e.g. Jane Appleseed" />
	</label>
	<label>
		Card Number
		<input type="text" placeholder="e.g. 1234 5678 9123 000" />
	</label>
	<label>
		Exp. Date (MM/YY)
		<input type="text" placeholder="MM" />
		<input type="text" placeholder="YY" />
	</label>
	<label>
		CVC
		<input type="number" placeholder="e.g. 123" />
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
		color: rgb(251, 242, 253);
		background-color: rgb(34, 9, 48);
	}

	input {
		border-radius: 5px;
		height: 40px;
		font-size: 1em;
		border-style: 1px solid gray;
	}

	label {
		display: flex;
		flex-direction: column;
		color: rgb(31, 20, 37);
	}
</style>
