<script>
import BigHeader from './component/BigHeader.svelte';
import data from './instagram.json';
import PhotoList from './component/PhotoList.svelte';

	export let hashtag;

</script>

<svelte:head>
  	<link href="https://cdnjs.cloudflare.com/ajax/libs/bulma/0.8.0/css/bulma.min.css" rel="stylesheet" />
</svelte:head>

<main class="container">
	<BigHeader hashtag = {hashtag} />
<input type="text" bind:value={hashtag} />
<h1>Photos</h1>
<PhotoList/>
</main>
