<script>
	import Logo from '$lib/components/logo.svelte';
	import DarkSwitch from '$lib/components/darkSwitch.svelte';
    import { onMount } from "svelte";

  onMount(() => {
    let lastScroll = 0;
    const nav = document.getElementById("navbar-sticky");
    document.getElementById("hero").style.height = nav.offsetHeight + "px";

    window.addEventListener("scroll", () => {
      const currentScroll = window.pageYOffset;

      if (currentScroll <= 0) {
        nav.classList.remove("show");
      }
      if (currentScroll > lastScroll && !nav.classList.contains("hidden")) {
        nav.classList.remove("show");
        nav.classList.add("hidden");
      }
      if (currentScroll < lastScroll && nav.classList.contains("hidden")) {
        nav.classList.remove("hidden");
        nav.classList.add("show");
      }
      lastScroll = currentScroll;
    });
  });
</script>

<nav class="fixed w-full bottom-0 top-auto z-10 sm:top-0 sm:bottom-auto" id="navbar-sticky">
	<div class="py-2 c-blur">
		<div class="container">
			<div class="flex justify-between content-center pr-3">
				<div class="flex flex-1 content-center">
					<div class=" grid content-center"><DarkSwitch /></div>
					<a class="content-center mx-2 hidden sm:grid" href="instagram.com/amartislab"><i class="fab fa-instagram" /></a>
					<a class="content-center mx-2 hidden sm:grid" href="facebook.com/amartislab"><i class="fab fa-facebook" /></a>
					<a class="content-center mx-2 hidden sm:grid" href="twitter.com/amartislab"><i class="fab fa-twitter" /></a>
					<a class="content-center mx-2 hidden sm:grid" href="wa.me"><i class="fab fa-whatsapp" /></a>
				</div>
				<div class="">
					<a class="navbar-brand" href="/">
						<!-- <img src="/img/logo.png" alt="Amartislab logo" /> -->
						<Logo/>
					</a>
				</div>
				<div class="flex flex-1 justify-end gap-2">
					<a href="/" class="uppercase hidden sm:grid content-center">Home</a>
					<a href="/about" class="uppercase hidden sm:grid content-center">About</a>
					<a href="/services" class="uppercase hidden sm:grid content-center">Services</a>
					<a href="/work" class="uppercase hidden sm:grid content-center">Work</a>
					<a href="/contact" class="uppercase hidden sm:grid content-center">Contact</a>
					<span id="menuToggle" class="uppercase sm:hidden grid content-center"><i class="fas fa-bars"></i></span>
				</div>
			</div>
		</div>
	</div>
</nav>

<style>
	#navbar-sticky .c-blur{
		backdrop-filter: blur(20px);
	}
</style>
