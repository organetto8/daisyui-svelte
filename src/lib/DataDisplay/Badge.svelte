<script lang='ts'>

    let userClass:string = '';
    let size:string = 'md';
    let color:string = '';

    let componentClass:string = [
        'badge',
        'badge-'+size,
        color !=='' ? 'badge-'+color : '',
        userClass
    ].join(' ');

    export { size, color, userClass as class };

</script>

<div class="{componentClass}"><slot/></div>