<script>
	import Footer from './../lib/footer.svelte';
	import Nav from './../lib/nav.svelte';
	import '../app.css';

</script>

<header>
    <Nav/>
</header>

<div id="root">
    <slot />
</div>
<Footer/>

