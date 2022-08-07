<script lang="ts">

    let userClass: string = '';
    let center: boolean = false;

    let componentClass: string = [
        'footer',
        center ? 'footer-center' : '',
        userClass
    ].join(' ');

    export { center, userClass as class }

</script>

<footer class="{componentClass}" {...$$restProps}>
    <slot/>
</footer>