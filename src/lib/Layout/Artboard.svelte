<script lang='ts'>

    let userClass: string = '';
    let phone: string = '';
    let demo: boolean = false;
    let horizontal: boolean = false;

    let componentClass: string = [
        'artboard',
        `phone-${phone}`,
        demo ? 'artboard-demo' : '',
        horizontal ? 'artboard-horizontal' : '',
        userClass
    ].join(' ');

    export { phone, demo, horizontal, userClass as class }

</script>

<div class="{componentClass}" {...$$restProps}>
    <slot/>
</div>