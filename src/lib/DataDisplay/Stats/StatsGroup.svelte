<script lang='ts'>

    let userClass: string = '';
    let vertical: boolean = false;
    let horizontal: boolean = true;

    let componentClass: string = [
        'stats',
        vertical ? 'stats-vertical' : 'stats-horizontal',
        userClass,
    ].join(' ')

    export { vertical, horizontal, userClass as class };

</script>

<div class="{componentClass}">
    <slot/>
</div>