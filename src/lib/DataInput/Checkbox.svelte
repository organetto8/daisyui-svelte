<script lang='ts'>

    let userClass: string = '';
    let color: string = '';
    let size: string = 'md';

    let componentClass: string = [
        'checkbox',
        color !== '' ? `checkbox-${color}` : '',
        `checkbox-${size}`,
        userClass
    ].join(' ')

    export { color, size, userClass as class }

</script>

<input type="checkbox" class='{componentClass}' {...$$restProps}/>