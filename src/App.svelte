<script>
	import DeviceList from './components/DeviceList.svelte'
	import Device from './components/Device.svelte'
	import Login from './components/login/loginPage.svelte'

	let headingMessage = 'Device List'
	let instructionMessage = 'Please select your desired device from the list below'
	let devices = [
		{
			id: '001cax',
			name: 'rPi2',
			connectionType: 'USB-A',
			idealSpeed: 200,
			realSpeed: 59,
			previouslyConnected: false,
			authorized: true
		},
		{
			id: '1033bs',
			name: 'raspberryPiTouchScreen3.1',
			connectionType: 'USB-C',
			idealSpeed: 480,
			realSpeed: 12,
			previouslyConnected: true,
			authorized: false
		}
	]
</script>

<main class="container">
	<!-- <div>
		<h1>
			{headingMessage}
		</h1>
		{instructionMessage}
	</div>
	<DeviceList {devices}/> -->

	<Login/>
</main>

<style>

</style>