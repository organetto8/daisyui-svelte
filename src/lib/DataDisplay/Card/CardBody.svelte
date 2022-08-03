<script lang="ts">
	let userClass: string = '';
	let componentClass: string = [
        'card-body',
        userClass
    ].join(' ');

    export { userClass as class };
</script>

<div class="{componentClass}">
    <slot/>
</div>