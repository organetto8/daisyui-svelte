<script lang="ts">

    let userClass: string = '';

    let componentClass: string = [
        'footer-title',
        userClass
    ].join(' ');

    export { userClass as class }

</script>

<span class="{componentClass}" {...$$restProps}>
    <slot/>
</span>