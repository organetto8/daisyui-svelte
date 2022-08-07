<script lang="ts">

    let userClass: string = '';
    let active: boolean = false;
    let hover: boolean = false;

    let componentClass: string = [
        active ? 'active' : '',
        hover ? 'hover' : '',
        userClass
    ].join(' ');

    export { active, hover, userClass as class };

</script>

<tr class="{componentClass}" {...$$restProps}>
    <slot/>
</tr>