<script lang='ts'>

    let userClass: string = '';
    let color: string = '';
    let size: string = 'md';

    let componentClass: string = [
        'radio',
        color !== '' ? `radio-${color}` : '',
        `radio-${size}`,
        userClass
    ].join(' ')

    export { color, size, userClass as class }

</script>

<input type="radio" class='{componentClass}' {...$$restProps}/>