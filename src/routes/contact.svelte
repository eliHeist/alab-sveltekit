<script>
	import Form1 from './../lib/components/forms/form1.svelte';
	import ContactCard from './../lib/components/contactCard.svelte';
</script>

<section class="">
	<div class="container-fluid">
		<div class="grid grid-cols-1 md:grid-cols-2 min-h-screen">
			<div class="pt-32 grid content-center">
				<div class="ml-auto w-fit p-8">
					<p class="text-xl py-2 font-light">
						Get in touch with us on the platforms indicated below 
					</p>
					<p class="text-xl py-2 font-light">
						or write to us here
					</p>
					<ol class="text-xl mt-4 font-light">
						<li class="my-1"><i class="fas fa-call mr-4" />+256 760 971 269</li>
						<li class="my-1"><i class="fas fa-envelope mr-4" />info@amartislab.com</li>
						<li class="my-1"><i class="fas fa-community mr-4" />@amartislab</li>
					</ol>
					<div class="flex">
						<a class="content-center mx-2" href="instagram.com/amartislab"><i class="fab fa-instagram" /></a>
						<a class="content-center mx-2" href="facebook.com/amartislab"><i class="fab fa-facebook" /></a>
						<a class="content-center mx-2" href="twitter.com/amartislab"><i class="fab fa-twitter" /></a>
						<a class="content-center mx-2" href="wa.me"><i class="fab fa-whatsapp" /></a>
						<a class="content-center mx-2" href="mailto:info.amartislan.com"><i class="fas fa-envelope" /></a>
					</div>
				</div>
			</div>
			<!-- form -->
			<div class="pt-32 dark:bg-dark-300 bg-white grid content-center">
				<div class=" p-12 h-full">
					<Form1 />
				</div>
			</div>
		</div>
	</div>
</section>

<style>
</style>
