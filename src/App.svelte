<script>
	import DeviceList from './components/DeviceList.svelte'
	import Device from './components/Device.svelte'

	let devices = [
		{
			id: '001cax',
			name: 'rPi2',
			connectionType: 'USB-A',
			speed: 200,
			previouslyConnected: false,
			authorized: true
		},
		{
			id: '1033bs',
			name: 'raspberryPiTouchScreen3.1',
			connectionType: 'USB-C',
			speed: 480,
			previouslyConnected: true,
			authorized: false
		}
	]
</script>

<main>
	<DeviceList {devices}/>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>