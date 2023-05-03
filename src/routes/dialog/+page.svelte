<script lang="ts">
	import { onMount } from 'svelte';

	let dialog: HTMLDialogElement;
	onMount(() => {
		dialog = document.getElementById('dialog') as HTMLDialogElement;
	});

	const showDialog = () => {
		dialog.showModal();
	};
</script>

<div class="flex items-center justify-center min-h-screen">
	<dialog id="dialog" class="card hidden">
		<div class="card-body">
			<div class="card-title">Die Dialog</div>
			<div class="card-text">
				Die <abbr>Dialog</abbr> ist ein HTML-Element, das als Modal verwendet werden kann. Es ist ein
				neues Element in HTML5.
			</div>
			<div class="card-actions justify-end">
				<button on:click={() => dialog.close()} class="btn btn-primary"> schließen </button>
			</div>
		</div>
	</dialog>
	<button on:click={showDialog} class="btn">Zeigen</button>
</div>

<style lang="postcss">
	#dialog[open] {
		@apply flex;
	}
</style>
