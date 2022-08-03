<script lang="ts">

    let size:string = 'h2';

    switch (size) {
        case '3xl':
            size = 'h1';
            break;
        case '2xl':
            size = 'h2';
            break;
        case 'xl':
            size = 'h3';
            break;
        case 'lg':
            size = 'h4';
            break;
        case 'md':
            size = 'h5';
            break;
        case 'sm':
            size = 'h6';
            break;
        case 'xs':
            size = 'h7';
            break;
        default:
            size = size
            break;
    }


    let userClass:string = '';
    let componentClass:string = [
        'card-title',
        userClass
    ].join(' ')

    export { size, userClass as class };

</script>

<svelte:element this='{size}' class="{componentClass}"><slot/></svelte:element>