<script lang="ts">
	let color: string = 'primary';
	let size: string = 'md';
	let ghost: boolean = false;
	let link: boolean = false;
	let outline: boolean = false;
	let active: boolean = false;
	let disabled: boolean = false;
	let glass: boolean = false;
	let loading: boolean = false;
	let noAnimation: boolean = false;
	let wide: boolean = false;
	let block: boolean = false;
	let circle: boolean = false;
	let square: boolean = false;

	let userClass: string = '';
	export {
		color,
		size,
		ghost,
		link,
		outline,
		active,
		disabled,
		glass,
		loading,
		noAnimation,
		circle,
		square,
		wide,
		block,
		userClass as class
	};

	let componentClass: string = [
		'btn',
		`btn-${color}`,
		`btn-${size}`,
		ghost ? 'btn-ghost' : '',
		link ? 'btn-link' : '',
		outline ? 'btn-outline' : '',
		active ? 'btn-active' : '',
		disabled ? 'btn-disabled' : '',
		wide ? 'btn-wide' : '',
		block ? 'btn-block' : '',
		glass ? 'glass' : '',
		loading ? 'loading' : '',
		noAnimation ? 'no-animation' : '',
		circle ? 'btn-circle' : '',
		square ? 'btn-square' : ''
	].join(' ');
</script>

<button class='{componentClass} {userClass}'>
	<slot/>
</button>
