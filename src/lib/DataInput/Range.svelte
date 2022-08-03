<script lang="ts">
	let userClass: string = '';
	let color: string = '';
	let size: string = 'md';
	let dashed: boolean = false;
    let min: string = '0';
    let max: string = '100';
    let step: string = '1';

	let componentClass: string = [
		'range',
		color !== '' ? `range-${color}` : '',
		`range-${size}`,
		userClass
	].join(' ');

	export { min, max, step, dashed, color, size, userClass as class };
</script>

<input type="range" {min} {max} {step} class={componentClass} {...$$restProps} />
{#if dashed}
	<div class="w-full flex justify-between text-xs px-2">
        {#each Array(Math.floor((Number(max)/Number(step)) + 1)) as _}        
            <span>|</span>
        {/each}
	</div>
{/if}
