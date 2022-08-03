<script lang="ts">
	let userClass: string = '';
	let componentClass: string = [
        'collapse-title',
        userClass
    ].join(' ');

    export { userClass as class };
</script>

<div class="{componentClass}"><slot/></div>
