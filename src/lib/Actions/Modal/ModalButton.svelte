<script lang='ts'>
    import { randomId } from "$lib/utils";

    let customId:string = randomId();
    let userClass:string = '';
    let component:string = 'btn'

    let componentClass:string = [
        component,
        'modal-button',
        userClass
    ].join(' ');

    export { customId as id };
    export { userClass as class };
    export { component };

</script>

<label for="{customId}" class='{componentClass}'><slot/></label>

<!-- Put this part before </body> tag -->
<input type="checkbox" id="{customId}" class="modal-toggle" />