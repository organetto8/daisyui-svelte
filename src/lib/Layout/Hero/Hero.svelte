<script lang="ts">

    let userClass: string = '';
    let overlay: string = '';

    let componentClass: string = [
        'hero',
        userClass
    ].join(' ');

    export { overlay, userClass as class }

</script>

<div class="{componentClass}" {...$$restProps}>
    {#if overlay !== ''}
        <div class="hero-overlay {overlay}"></div>
    {/if}
    <slot/>
</div>