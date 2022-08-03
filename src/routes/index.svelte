<script>
	import SimageCard from './../lib/components/simageCard.svelte';
	import Counter from './../lib/components/counter.svelte';
	import PolyButton from './../lib/components/polyButton.svelte';

</script>

<!-- hero section -->
<section class="bg-white dark:bg-black">
    <div id="hero"></div>
    <div class="container grid justify-center py-72">
        <h1 class="uppercase text-7xl font-bold text-center">Your Brand, Your Story</h1>
        <div class="grid sm:grid-cols-3 gap-4 mx-auto text-center mt-10">
            <PolyButton text="Services" link="/services" cls="primary"/>
            <PolyButton text="Work" link="/work"/>
            <PolyButton text="Contact" link="/contact"/>
        </div>
    </div>
</section> <!--end hero-->

<!-- about -->
<section class="py-5 my-40">
        <h2 class="uppercase text-6xl font-bold text-center">Who are we?</h2>

    <div class="grid sm:grid-cols-2 md:grid-cols-2 mt-12 container">
        <!-- achievements -->
        <div class="flex justify-end">
            <div class="grid grid-cols-2 gap-4 w-full">
                <!-- cards here -->
                <Counter number="20" text="Satisfied Customers"/>
                <Counter number="50" text="Designs Made"/>
                <Counter number="20" text="Videos Produced"/>
                <Counter number="20" text="Satisfied Customers"/>
            </div>
        </div>
        <!-- about us -->
        <div>
            <p class="sm:ml-6 mt-8 max-w-xl lead text-center sm:text-left">
                Amarti's lab is a next generation agency delivering brand design, web development, animation
				and visual effects. Our agile agency model is built on an extensive network of highly
				talented strategic and creative professionals who work collaboratively with clients
				worldwide to meet their business objectives.
            </p>
        </div>
    </div>
</section>

<!-- What we do -->
<section class="py-5 my-40">
    <h2 class="header-1">What do we do?</h2>
    <div class="container mt-12">
        <!-- cards go here -->
        <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
            <SimageCard/>
            <SimageCard/>
            <SimageCard/>
            <SimageCard/>
        </div>
    </div>
</section>

<!-- featured projects -->
<section class="py-5 my-40">
    <h2 class="header-1">Our featured work</h2>
    <div class="container mt-12">
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
            <div class=" aspect-square">
                <img src="/img/projects/2.jpg" alt="" class=" object-cover">
            </div>
            <div class=" aspect-square">
                <img src="/img/projects/7.jpg" alt="" class=" object-cover">
            </div>
            <div class=" aspect-square">
                <img src="/img/projects/8.jpg" alt="" class=" object-cover">
            </div>
            <div class=" aspect-square">
                <img src="/img/projects/9.jpg" alt="" class=" object-cover">
            </div>
            <div class=" aspect-square">
                <img src="/img/projects/22.jpg" alt="" class=" object-cover">
            </div>
            <div class=" aspect-square">
                <img src="/img/projects/26.jpg" alt="" class=" object-cover">
            </div>
            <div class=" aspect-square">
                <img src="/img/projects/36.jpg" alt="" class=" object-cover">
            </div>
            <div class=" aspect-square">
                <img src="/img/projects/52.jpg" alt="" class=" object-cover">
            </div>
        </div>
    </div>
</section>

<!-- clients -->
<section class="py-5 my-40">
    <h2 class="header-1">Our notable clients</h2>
    <div class="container mt-12">
        <div class="grid grid-cols-2 xl:grid-cols-5 gap-4 justify-center">
            <div class=" h-28 aspect-video grid place-content-center p-3">
                <img src="/img/clients/drach-concepts.png" alt="MBF" class=" fluid">
            </div>
            <div class=" h-28 aspect-video bg-gray-100 grid place-content-center p-3">
                <img src="/img/clients/mbf autos.png" alt="MBF" class=" fluid">
            </div>
            <div class=" h-28 aspect-video bg-gray-100 grid place-content-center p-3">
                <img src="/img/clients/paries bakery.png" alt="MBF" class=" fluid">
            </div>
            <div class=" h-28 aspect-video bg-gray-100 grid place-content-center p-3">
                <img src="/img/clients/queen of peace.png" alt="MBF" class=" fluid">
            </div>
            <div class=" h-28 aspect-video grid place-content-center p-3">
                <img src="/img/clients/UNESCO.png" alt="MBF" class=" fluid">
            </div>
        </div>
    </div>
</section>

<!-- testimonials -->
<section class="py-5 my-40">
    <h2 class="header-1">What they say about us</h2>
    <div class="container mt-12">
        <div class="grid sm:grid-cols-2 md:grid-cols-3 md:grid-rows-2 gap-4">
            <div class=" flex flex-col p-8 bg-slate-300 dark:bg-slate-900 sm:col-span-2 md:col-span-1 lg:row-span-2">
                <p class=" flex-1">
                    Professional Website Design: Webstar is committed to better website designs and the best web hosting packages in Uganda. The websites are mobile use friendly and search indexed to appear on Google's first page
                </p>
                <i class="mb-0 ml-auto pt-8 text-sm">~ John Doe, CEO Nothing</i>
            </div>
            <div class=" flex flex-col p-8 bg-slate-300 dark:bg-slate-900">
                <p class=" flex-1">
                    Professional Website Design: Webstar is committed to better website designs and the best web hosting packages in Uganda. The websites are mobile use friendly and search indexed to appear on Google's first page
                </p>
                <i class="mb-0 ml-auto pt-8 text-sm">~ John Doe, CEO Nothing</i>
            </div>
            <div class=" flex flex-col p-8 bg-slate-300 dark:bg-slate-900">
                <p class=" flex-1">
                    Professional Website Design: Webstar is committed to better website designs and the best web hosting packages in Uganda. The websites are mobile use friendly and search indexed to appear on Google's first page
                </p>
                <i class="mb-0 ml-auto pt-8 text-sm">~ John Doe, CEO Nothing</i>
            </div>
            <div class=" flex flex-col p-8 bg-slate-300 dark:bg-slate-900">
                <p class=" flex-1">
                    Professional Website Design: Webstar is committed to better website designs and the best web hosting packages in Uganda. The websites are mobile use friendly and search indexed to appear on Google's first page
                </p>
                <i class="mb-0 ml-auto pt-8 text-sm">~ John Doe, CEO Nothing</i>
            </div>
            <div class=" flex flex-col p-8 bg-slate-300 dark:bg-slate-900 md:col-span-2 lg:col-span-1">
                <p class=" flex-1">
                    Professional Website Design: Webstar is committed to better website designs and the best web hosting packages in Uganda. The websites are mobile use friendly and search indexed to appear on Google's first page
                </p>
                <i class="mb-0 ml-auto pt-8 text-sm">~ John Doe, CEO Nothing</i>
            </div>
        </div>
    </div>
</section>
