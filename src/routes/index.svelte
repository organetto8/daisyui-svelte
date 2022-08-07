<script lang="ts">
	import { Button, Modal, ModalAction, ModalBox, ModalButton, Dropdown, DropdownContent } from '$lib';
	import { Alert, Avatar, AvatarGroup, Collapse, CollapseContent, CollapseTitle, Countdown, Badge, Kbd, Card, CardBody, CardImage, CardTitle, Progress, RadialProgress, Stat, StatDesc, StatFigure, StatTitle, StatValue, StatsGroup } from '$lib';
	import { Checkbox, FormControl, Radio, Range, Rating, Select, TextInput, Toggle } from '$lib';
	import { Mask } from '$lib';

	let value: number = 10;

	setInterval(() => {
		value > 0 ? value-- : (value = 10);
	}, 1000);
</script>

<main class="space-y-15">
	<Button>Mammt</Button>

	<div class="flex gap-2 items-center">
		<Kbd>Ctrl</Kbd>+
		<Kbd>Shift</Kbd>+
		<Kbd>F</Kbd>
	</div>

	<Alert color="error" class="text-white">Mammt Annur Fa E Bucchin</Alert>

	<div class="flex flex-col space-y-5">
		<Countdown {value} />

		<Badge color="success">Par O Cazz</Badge>
	</div>

	<Card class="w-1/4 shadow-xl bg-success">
		<CardBody>
			<CardTitle>Mammt Annur UeUe</CardTitle>
			<p class="content">Par pop e pall frate</p>
		</CardBody>
	</Card>

	<Collapse button="arrow" class="rounded-2xl border bg-info">
		<CollapseTitle>Mammt Annur UeUe</CollapseTitle>
		<CollapseContent>
			<p>Par pop e pall frate</p>
		</CollapseContent>
	</Collapse>

	<Progress value="20" max="100" color="success" class="w-1/4" />
	<Progress color="success" class="w-1/4" />

	<RadialProgress value="20" textColor="primary-content" backgroundColor="primary" />

	<StatsGroup class="bg-primary text-primary-content">
		<Stat>
			<StatTitle>Mammt Annur UeUe</StatTitle>
			<StatValue>Par pop e pall frate</StatValue>
			<StatDesc>Le Pallissime proprio</StatDesc>
		</Stat>
		<Stat>
			<StatTitle>Mammt Annur UeUe</StatTitle>
			<StatValue>Par pop e pall frate</StatValue>
			<StatDesc>Le Pallissime proprio</StatDesc>
		</Stat>
		<Stat>
			<StatTitle>Mammt Annur UeUe</StatTitle>
			<StatValue>Par pop e pall frate</StatValue>
			<StatDesc>Le Pallissime proprio</StatDesc>
		</Stat>
	</StatsGroup>

	<Checkbox color="primary" size="lg" checked />

	<TextInput value='Mammt' placeholder='Papara?' bordered color='primary' size='lg'>
        <h1>Papara?</h1>
    </TextInput>

    <Radio name='papara' color='primary' size='lg' checked></Radio>
    <Radio name='papara' color='primary' size='lg' ></Radio>

    <Range min="0" max="100" step="50" color="primary" size="lg" dashed/>

    <Rating max="5" value='2' shape="heart"/>

	<Mask>
		<img src="https://placeimg.com/160/160/arch" alt="mammt"/>
	</Mask>

</main>
