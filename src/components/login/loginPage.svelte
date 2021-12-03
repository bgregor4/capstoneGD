<script>
    async function submit(event) {
		const response = await post(`insert auth wrapper class file location`, { username, password });
	}

    let username = "";
    let password = "";
</script>

<div>
    <h1 class="welcomeHeading">
        Welcome to the Raspberry Pi Device Management Tool
    </h1>
    <form on:submit|preventDefault={submit} class="form">
        <fieldset class="fieldsetClass">
            <input class="form-input" required placeholder="Username" bind:value={username}>
        </fieldset>
        <fieldset class="fieldsetClass">
            <input class="form-input" type="password" required placeholder="Password" bind:value={password}>
        </fieldset>
        <button class="button" type="submit">
            Submit Login information
        </button>
    </form>
</div>

<style>
    .welcomeHeading {
        text-align: center;
    }

    .fieldsetClass {
        margin: 0 auto;
        border: none;
        padding: 5px 0;
        max-width: 30%;
    }

    .form-input {
        height: 25px;
        max-width: 100%;
    }
</style>