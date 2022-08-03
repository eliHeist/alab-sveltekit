<script>
	export let label = 'Label here';
	export let type = 'text';
	export let name = '';
	export let required = 'required';
</script>

<div class="input-group">
	<input {required} {type} {name} class="input dark:bg-dark-100 dark:text-white text-black bg-light-200" />
	<label class="user-label dark:text-white text-black" for={name}>{label}</label>
</div>

<style>
	/* From uiverse.io by @alexruix */
	.input-group {
		position: relative;
	}

	.input {
		@apply text-base p-4;
		border-radius: 1rem;
		transition: border 150ms cubic-bezier(0.075, 0.82, 0.165, 1);
		width: 100%;
	}

	.user-label {
		@apply absolute;
		left: 15px;
		pointer-events: none;
		transform: translateY(1rem);
		transition: 150ms cubic-bezier(0.4, 0, 0.2, 1);
	}

	.input:focus,
	input:valid {
		@apply border border-solid border-primary-900;
		outline: none;
	}

	.input:focus ~ label,
	input:valid ~ label {
		@apply text-white font-semibold bg-primary-900;
		transform: translateY(-50%) scale(0.8);
		padding: 0 0.2em;
	}
</style>
