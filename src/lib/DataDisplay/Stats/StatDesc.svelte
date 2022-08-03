<script lang='ts'>

    let userClass: string = '';

    let componentClass: string = [
        'stat-desc',
        userClass
    ].join(' ')

    export { userClass as class }
</script>

<div class="{componentClass}">
    <slot/>
</div>