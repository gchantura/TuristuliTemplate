<script>
	import Navbar from '../components/Navbar/Navbar.svelte';
	import '../app.css';

	import Footer from '../components/Footer/Footer.svelte';
</script>

<div class="navbar">
	<Navbar />
</div>

<div class="content dark:bg-slate-400">
	<slot />
</div>

<div class="footer"><Footer /></div>
