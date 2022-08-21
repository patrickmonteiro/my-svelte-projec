<script lang="ts">
	export let name: string;
	export const description: string = 'Essa é uma descrição';
	export const src: string = 'https://cdn.pixabay.com/photo/2014/10/30/21/41/tutankhamun-509752_1280.jpg';
	export const alt: string = 'Egito'
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>{description}</p>
	<img {src} {alt} height="300px">
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