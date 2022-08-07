<script lang="ts">

    let userClass: string = '';

    let componentClass: string = [
        'hero-content',
        userClass
    ].join(' ');

    export { userClass as class }
</script>

<div class="{componentClass}" {...$$restProps}>
    <slot/>
</div>