<!-- <script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<h1>
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src={welcome_fallback} alt="Welcome" />
			</picture>
		</span>

		to your new<br />SvelteKit app
	</h1>

	<h2>
		try editing <strong>src/routes/+page.svelte</strong>
	</h2>

	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style> -->



<script>
    // import { version } from "vite";
    import App from "./App.svelte";
    import Await from "./Await.svelte";
    import Dom from "./dom.svelte";
    import Each from "./Each.svelte";
    import EventModifiers from "./EventModifiers.svelte";
    import GroupsInput from "./GroupsInput.svelte";
    // import Info from "./info.svelte";
    // import Nested from "./Nested.svelte";
    import Ifelse from "./Ifelse.svelte";
    import InlineHandlers from "./InlineHandlers.svelte";
    import Inner from "./Inner.svelte";
    import Input from "./Input.svelte";

	// const pkg = {
	// 	name: 'svelte',
	// 	version : '3',
	// 	speed: 'blazing',
	// 	website: 'https://svelte.dev'

	// }
function handleMessage(e){
	alert(e.detail.text)
}

</script>

<section>
	<!-- <App/> -->
	<!-- <Nested answer = {42}/> -->
	<!-- <Nested/> -->

	<!-- <Info {...pkg} /> -->
	 <!-- <Ifelse/> -->
	  <!-- <Each/> -->
	   <!-- <Await/> -->
		<!-- <Dom/> -->
	<!-- <InlineHandlers/> -->
	<!-- <EventModifiers/> -->
	
	<!--  -->
<!-- <Inner on:message={handleMessage}/> -->
 <!-- <Input/> -->
<GroupsInput/>
	
</section>
