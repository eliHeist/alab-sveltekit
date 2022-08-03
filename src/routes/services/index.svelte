<script>
	import Link from '$lib/components/link.svelte';

    // reverse classes to toggle
    let reverse = '-reverse';
    let ml = 'ml-auto'
</script>

<section class="py-60">
<h1 class="uppercase text-7xl font-bold text-center">What do we do?</h1>
</section>
<section>
    <div class="container-full">
        <div class="flex flex-col sm:flex-row my-40">
            <figure class=" flex-1 w-full overflow-hidden max-h-96">
                <img src="/img/projects/2.jpg" alt="" class="object-cover w-full h-full" />
            </figure>
            <div class="flex-1 grid content-center p-4">
                <div class="max-w-xl ">
                    <h2 class="header-2">Graphics design</h2>
                    <p class="lead mt-8">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nemo quo sit laborum! Deserunt
                        iure aliquid nam cum exercitationem commodi magnam voluptatem dicta quam. Est, tempore.
                        Earum natus aperiam magni eaque!
                    </p>
                    <div class=" mt-12">
                        <Link href="/services/1" text="View Packages" />
                    </div>
                </div>
            </div>
        </div>
        <!-- card to loop -->
        <div class="flex flex-col sm:flex-row{reverse} my-40">
            <figure class=" flex-1 w-full overflow-hidden max-h-96">
                <img src="/img/projects/2.jpg" alt="" class="object-cover w-full h-full" />
            </figure>
            <div class="flex-1 grid content-center p-4">
                <div class="max-w-xl {ml}">
                    <h2 class="header-2">Graphics design</h2>
                    <p class="lead max-w-xl mt-8">
                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nemo quo sit laborum! Deserunt
                        iure aliquid nam cum exercitationem commodi magnam voluptatem dicta quam. Est, tempore.
                        Earum natus aperiam magni eaque!
                    </p>
                    <div class=" mt-12">
                        <Link href="/services/1" text="View Packages" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
