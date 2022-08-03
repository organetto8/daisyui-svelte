<script lang="ts">
	let userClass: string = '';
    let color: string = '';
    let value: string = '';
    let max: string = '';
    let componentValue: string;
    let componentClass: string = [
        'progress',
        color !=='' ? `progress-${color}` : '',
        userClass
    ].join(' ');

    export { color, value, max, userClass as class };
</script>

{#if value !== ''}
    <progress class="{componentClass}" {value} {max}><slot/></progress>
{/if}
{#if value !== ''}
    <progress class="{componentClass}" {max}><slot/></progress>
{/if}