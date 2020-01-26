<script>
	export let name;
	const familyName = 'Lanese';

	function changeName() {
		name = (name === 'Leo')?  'Leonardo' : 'Leo';
	}
</script>

<style>
	h1 {
		color: darkred;
	}
</style>

<h1>Hello, my name is: {name} {familyName}</h1>
<button on:click={changeName}>Change-Name</button>
