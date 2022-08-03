<script>
	import PackageCard from './../../lib/components/packageCard.svelte';
</script>

<section class="banner">
    <div id="hero"></div>
    <div class="py-32">
        <h1 class="header-1">Graphics</h1>
    </div>
</section>
<!-- packages -->
<section>
    <div class="container mt-16">
        <h2 class="w-min text-6xl uppercase">Logo <span class="text-primary-500 font-extrabold">Packages</span></h2>
        <div class="flex gap-6 mt-12 justify-center grid-auto">
            <PackageCard/>
            <PackageCard/>
            <PackageCard/>
            <!-- <div class="package-card mt-6 sm:max-w-sm text-center">
                <header class=" p-4 bg-primary-500">
                    <span class=" text-5xl font-bold">70K</span>
                </header>
                <div class="p-4">
                    <p class="lead">
                        For those who need a low resolution file as inspiration for their designer.
                    </p>
                </div>
                <hr class=" w-3/4 mx-auto border-slate-500" />
                <div class="p-4">
                    <div class="flex w-full justify-center">
                        1 Logo file
                    </div>
                </div>
            </div>
            <div class="package-card mt-6 sm:max-w-sm text-center">
                <header class=" p-4 bg-primary-500">
                    <span class=" text-5xl font-bold">500K</span>
                </header>
                <div class="p-4 border-x-2 border-slate-900">
                    <p class="lead">
                        For those who want an expert graphic designer to perfect their logo design.
                    </p>
                </div>
                <hr class=" w-3/4 mx-auto border-slate-500" />
                <div class="p-4 border-b-2 border-x-2 border-slate-900">
                    <div class="flex w-full justify-center py-3 border-b-2 border-slate-900">
                        everything in the premium
                    </div>
                    <div class="flex w-full justify-center py-3 border-b-2 border-slate-900">
                        time with the designer
                    </div>
                    <div class="flex w-full justify-center py-3 border-b-2 border-slate-900">
                        1 logo animation
                    </div>
                </div>
            </div> -->
        </div>
    </div>
</section>

<style>
    section.banner{
        background-image: url('/img/projects/2.jpg');
        background-size: cover;
        background-attachment: fixed;
        background-position: 50% 50%;
    }
    .grid-auto{
        grid-template-columns: repeat(auto-fit, minmax(20rem, 500px));
    }
</style>