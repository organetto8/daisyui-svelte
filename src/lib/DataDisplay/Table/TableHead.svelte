<script lang="ts">

    let userClass: string = '';

    export { userClass as class };
</script>

<th class="{userClass}" {...$$restProps}>
    <slot/>
</th>