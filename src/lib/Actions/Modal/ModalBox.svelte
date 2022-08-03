<script lang='ts'>

    let customClass:string = '';

    export { customClass as class }

</script>

<div class="modal-box {customClass}">
    <slot/>
</div>