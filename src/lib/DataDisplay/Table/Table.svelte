<script lang="ts">

    let userClass: string = '';
    let compact: boolean = false;
    let normal: boolean = false;
    let zebra: boolean = false;
    let componentClass: string = [
        'table',
        compact ? 'table-compact' : '',
        normal ? 'table-normal' : '',
        zebra ? 'table-zebra' : '',
        userClass
    ].join(' ')

    export { userClass as class, compact, normal, zebra};

</script>

<table class="{componentClass}" {...$$restProps}>
    <slot/>
</table>