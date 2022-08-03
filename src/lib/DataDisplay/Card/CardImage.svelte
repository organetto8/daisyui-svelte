<script lang="ts">

    let source:string = '';
    let alternative:string = '';
    let userClass
    let componentClass:string = [
        userClass,
    ].join(' ')

    export { source as src, alternative as alt, userClass as class };

</script>



<figure class="{componentClass}"><img src="{source}" alt="{alternative}"/></figure>