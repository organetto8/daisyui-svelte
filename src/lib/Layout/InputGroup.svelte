<script lang='ts'>

    let userClass: string = '';
    let vertical: boolean = false;
    let size: string = 'md';

    let componentClass: string = [
        'btn-group',
        `btn-group-${size}`,
        vertical ? 'btn-group-vertical' : '',
        userClass
    ].join(' ');

    export { vertical, size, userClass as class }

</script>

<label class="{componentClass}" {...$$restProps}>
    <slot/>
</label>