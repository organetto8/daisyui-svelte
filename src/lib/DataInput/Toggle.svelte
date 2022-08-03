<script lang='ts'>

    let userClass: string = '';
    let color: string = '';
    let size: string = 'md';

    let componentClass: string = [
        'toggle',
        color !== '' ? `toggle-${color}` : '',
        `toggle-${size}`,
        userClass
    ].join(' ')

    export { color, size, userClass as class }

</script>

<input type="checkbox" class='{componentClass}' {...$$restProps}/>