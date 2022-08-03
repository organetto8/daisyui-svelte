<script lang='ts'>

    let userClass: string = '';
    let value: string = '0';
    let size: string = '';
    let thickness: string = '';
    let textColor: string = '';
    let backgroundColor: string = '';
    
    let componentClass: string = [
        'radial-progress',
        textColor !== '' ? `text-${textColor}` : '',
        backgroundColor !== '' ? `bg-${backgroundColor}` : '',
        userClass
    ].join(' ');


    let componentStyle: string = [
        `--value:${value};`,
        size !=='' ?`--size:${size};` : size,
        thickness !=='' ?`--thickness:${thickness};` : thickness,
    ].join(' ')


    export { textColor, backgroundColor, value, size, thickness, userClass as class };

</script>

<div class="{componentClass}" style="{componentStyle}">{value}%</div>