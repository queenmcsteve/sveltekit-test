<script>
	const date = new Date();
	let name = "";
	let email = "";

	function handleClick() {
		window.open("https://static.esmt.org/pub/edtech/riseAnalyticsTest/index.html", '_blank');
		}

</script>

<!-- https://script.google.com/macros/s/AKfycbwlXnXGK4b1jfeZ2UHx8UtqeefonhQwQenbzr3m59WEjans5Xt9EK-WYxsi_wLvhJAA/exec -->
<!-- https://static.esmt.org/pub/edtech/riseAnalyticsTest/index.html -->



<main>
	<form target="_top" id="emailForm" method="POST" action="https://script.google.com/macros/s/AKfycbwlXnXGK4b1jfeZ2UHx8UtqeefonhQwQenbzr3m59WEjans5Xt9EK-WYxsi_wLvhJAA/exec">
		<p style="color: {email}">Please enter your name and email to access the SSK</p>
		<input name="date" type="text" value={date} hidden>
		name: <input name="name" type="text" bind:value={name} required>
		<br>
		email: <input name="email" type="email" bind:value = {email} required>
		<br>
		<button type="submit" on:click={handleClick}>
			submit
		</button>
	</form>
	
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