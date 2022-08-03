<script lang="ts">

    let color:string = '';
    let userClass:string = '';
    let bordered:boolean = false;
    let full:boolean = false;
    let side:boolean = false;
    let compact:boolean = false;

	let componentClass: string = [
        'card',
        bordered ? 'card-bordered' : '',
        color !== '' ? `bg-${color}` : color,
        compact ? 'card-compact' : '',
        full ? 'image-full' : '',
        side ? 'card-side' : '',
        userClass
    ].join(' ');

    export { full, side, compact, bordered, userClass as class };

</script>

<div class="{componentClass}"><slot/></div>