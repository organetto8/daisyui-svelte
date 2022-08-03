<script lang="ts">
	let userClass: string = '';
    let button: string = '';
    let status: string = '';

    let componentClass: string = [
        'collapse',
        `collapse-${button}`,
        status !== '' ? `collapse-${status}`: '',
        userClass
    ].join(' ');

    export { button, status, userClass as class };
</script>

<div class="{componentClass}">
    <input type="checkbox">
    <slot/>
</div>