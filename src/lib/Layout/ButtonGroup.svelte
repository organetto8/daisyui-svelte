<script lang='ts'>

    let userClass: string = '';
    let vertical: boolean = false;

    let componentClass: string = [
        'btn-group',
        vertical ? 'btn-group-vertical' : '',
        userClass
    ].join(' ');

    export { vertical, userClass as class }

</script>

<div class="{componentClass}" {...$$restProps}>
    <slot/>
</div>