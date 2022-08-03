<script lang="ts">
	let userClass: string = '';
    let size: string = 'md';
	let componentClass: string = [
        'kbd',
        `kbd-${size}`,
        userClass
    ].join(' ');

    export { userClass as class };
</script>

<kbd class="{componentClass}"><slot/></kbd>