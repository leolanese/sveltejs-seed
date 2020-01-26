<script>
	export let name;
	const familyName = 'Lanese';

	$: uppercaseName = name.toUpperCase();
	$: uppercaseFamilyName = familyName.toUpperCase();
	$: console.log(uppercaseName, uppercaseFamilyName);

	const changeName = () => name = (name === 'Leo')?  'Leonardo'  : 'Leo';
</script>

<style>
	h1 {
		color: #323f7d;
	}
	button {
		border: 1px solid #323f7d;
	}
</style>

<h1>Hello,  my name is: {uppercaseName} {uppercaseFamilyName}</h1>
<button on:click={changeName}>Change-Name</button>

