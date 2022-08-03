<script lang='ts'>

    export let align: string;
    export let direction: string;
    export let hover: boolean;
    export let open: boolean;

    let className = [
        'dropdown',
        align ? `dropdown-${align}` : '',
        direction ? `dropdown-${direction}` : '',
        hover ? 'dropdown-hover' : '',
        open ? 'dropdown-open' : '',
    ].join(' ');

</script>

<div class='{className}'>
    <slot/>
</div>