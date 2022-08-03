<script lang='ts'>

    let userClass: string = '';

    let componentClass = [
        'form-control',
        userClass
    ].join(' ');

    export { userClass as class }
</script>

<div class="{componentClass}"><slot/></div>