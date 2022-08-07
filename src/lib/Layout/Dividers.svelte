<script lang="ts">

    let userClass: string = '';
    let vertical: boolean = true;
    let horizontal: boolean = false;
    let componentClass: string = [
        'divider',
        vertical ? 'divider-vertical' : '',
        horizontal ? 'divider-horizontal' : '',
        userClass
    ].join(' ');

    export { vertical, horizontal, userClass as class }    

</script>

<div class="{componentClass}" {...$$restProps}>
    <slot/>
</div>