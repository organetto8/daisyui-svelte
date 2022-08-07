<script lang="ts">

    let userClass: string = '';

    export { userClass as class };

</script>

<td class="{userClass}" {...$$restProps}>
    <slot/>
</td>