<script>
    import DeviceDisplay from './DeviceDisplay.svelte'
    import DeviceList from './DeviceList.svelte';
    export let device
</script>

<DeviceDisplay>
    <div class="close">X</div>
    <div class="infoContainer">
        <div class="infoDisplay">
            <ul>
                <li>Device: {device.name}
                <li>ID: {device.id}
                <li>Connection Type: {device.connectionType}
                <li>Max potential speed: {device.idealSpeed}
                <li>Observed speed: {device.realSpeed}
                <li>Previous Connection: {device.previouslyConnected}
                <li>Authorized Device: {device.authorized}
            </ul>
        </div>
    </div>
    <button class="button">
        Select
    </button>

</DeviceDisplay>

<style>
    .close {
        position: absolute;
        top: 10px;
        right: 20px;
        cursor: pointer;
        background: none;
        border: none;
    }

    .infoContainer {


    }

    .infoDisplay {

    }

</style>