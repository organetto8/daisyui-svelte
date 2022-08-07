<script lang="ts">

    let userClass: string = '';
    let componentClass: string = [
        'indicator-item',
        userClass
    ].join(' ');

    export { userClass as class }

</script>

<div class="{componentClass}" {...$$restProps}>
    <slot/>
</div>