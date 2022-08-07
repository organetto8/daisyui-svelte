<script lang='ts'>
    import { randomId } from "$lib/utils";

    let color: string = '';
    let bordered: boolean = false;
    let ghost: boolean = false;
    let userClass: string = '';
    let id: string = randomId();

    let componentClass: string = [
        'textarea',
        bordered ? 'textarea-bordered' : '',
        ghost ? 'textarea-ghost' : '',
        color !== '' ? `textarea-${color}` : '',
        userClass
    ].join(' ');

    export { id, color, bordered, ghost, userClass as class};

</script>

<div class="">
    <input type="text" id={id} class='{componentClass}' {...$$restProps}>
</div>