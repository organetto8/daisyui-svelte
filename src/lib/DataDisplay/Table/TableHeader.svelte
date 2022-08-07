<script lang="ts">

    let userClass: string = '';

    export { userClass as class };

</script>

<thead class="{userClass}" {...$$restProps}>
    <slot/>
</thead>