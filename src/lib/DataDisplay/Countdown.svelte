<script lang="ts">
	let userClass: string = '';
    let value: number;
	let componentClass: string = [
        'countdown',
        userClass
    ].join(' ');

    export { value, userClass as class };
</script>

<span class="{componentClass}">
	<span style="--value:{value.toString()};" />
</span>
