<script lang='ts'>
    import { randomId } from "$lib/utils";

    let color: string = '';
    let size: string = 'md';
    let bordered: boolean = false;
    let ghost: boolean = false;
    let userClass: string = '';
    let id: string = randomId();

    let componentClass: string = [
        'select',
        `select-${size}`,
        bordered ? 'select-bordered' : '',
        ghost ? 'select-ghost' : '',
        color !== '' ? `select-${color}` : '',
        userClass
    ].join(' ');

    export { id, color, size, bordered, ghost, userClass as class};

</script>

<div class="">
    <select id={id} class='{componentClass}' {...$$restProps}>
        <slot/>
    </select>
</div>