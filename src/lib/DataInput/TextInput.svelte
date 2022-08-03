<script lang='ts'>
    import { randomId } from "$lib/utils";

    let color: string = '';
    let size: string = 'md';
    let bordered: boolean = false;
    let ghost: boolean = false;
    let userClass: string = '';
    let id: string = randomId();

    let componentClass: string = [
        'input',
        `input-${size}`,
        bordered ? 'input-bordered' : '',
        ghost ? 'input-ghost' : '',
        color !== '' ? `input-${color}` : '',
        userClass
    ].join(' ');

    export { id, color, size, bordered, ghost, userClass as class};

</script>

<div class="">
    <slot/>
    <input type="text" id={id} class='{componentClass}' {...$$restProps}>
</div>