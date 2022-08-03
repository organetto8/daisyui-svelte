<script lang='ts'>

    let max: string = '5';
    let shape: string = 'star';
    let value: string = '0';

    export { max, shape, value }

</script>

<div class="rating">
    {#each Array(parseInt(max)-1) as _, i}
        {#if i === parseInt(value)-1}
            <input type="radio" name="rating-7" checked class="mask mask-{shape}" />
        {/if}
        <input type="radio" name="rating-7" class="mask mask-{shape}" />
    {/each}
</div>