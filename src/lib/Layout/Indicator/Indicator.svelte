<script lang="ts">

    let userClass: string = '';
    let verticalSlot: string = 'top';
    let horizontalSlot: string = 'end';
    let componentClass: string = [
        'indicator',
        `indicator-${verticalSlot}`,
        `indicator-${horizontalSlot}`,
        userClass
    ].join(' ');

    export { verticalSlot, horizontalSlot, userClass as class }
</script>

<div class="{componentClass}" {...$$restProps}>
    <slot/>
</div>