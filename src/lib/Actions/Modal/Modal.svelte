<script lang="ts">

    export let bottom: string = '';
    export let middle: string = '';

	let userClass: string = '';

    let componentClass:string = [
        'modal',
        userClass,
        bottom ? `${bottom}:modal-bottom` : '',
        middle ? `${middle}:modal-middle` : '',
    ].join(' ');

	export { userClass as class };
</script>

<div class="modal {componentClass}">
	<slot />
</div>
