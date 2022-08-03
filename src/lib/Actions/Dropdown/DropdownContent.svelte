<svelte:element this={element} class="dropdown-content">
    <slot></slot>
</svelte:element>

<script lang='ts'>
    export let element: string;
</script>