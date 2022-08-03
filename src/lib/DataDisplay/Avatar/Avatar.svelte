<script lang="ts">
	let userClass: string;
	let online: boolean = false;
	let placeholder: string;

	export { userClass as class };
</script>

{#if !placeholder}
	<div class="avatar {userClass}" />
{:else}
	<div class="avatar placeholder">
		<div class="bg-neutral-focus text-neutral-content rounded-full w-24">
			<span class="text-3xl">K</span>
		</div>
	</div>
{/if}
