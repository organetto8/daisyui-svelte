<script lang="ts">

    let userClass: string = '';

    export { userClass as class };
</script>

<tbody class="{userClass}" {...$$restProps}>
    <slot/>
</tbody>