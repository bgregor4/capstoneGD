<script>
    import Device from './Device.svelte'
    export let devices = []
</script>

{#each devices as dev (dev.id)}
    <Device device={dev} />
{/each}