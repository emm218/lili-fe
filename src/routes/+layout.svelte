<script>
	import "../app.css";
	import { Modals, closeModal } from 'svelte-modals'
</script>

<Modals>
	<div slot="backdrop" class="fixed top-0 left-0 w-full h-full bg-black/25"
		on:click={closeModal}
	/>
</Modals>

<slot />
