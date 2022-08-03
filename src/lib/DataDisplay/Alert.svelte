<script lang="ts">
	let userClass: string = '';
	let componentClass: string;
	let color: string = '';
    color !== '' ? componentClass = `alert-${color}` : componentClass = '';
	export { color, userClass as class };
</script>

<div class="alert {componentClass} {userClass}">
	<slot />
</div>