<script>
	import Arrow from './arrow.svelte';
    let title = 'Basic'
    let ammount = '450000'
    let mainDigits
    let zeroes
    function getlength(ammount) {
        return ammount.toString().length
    }

    const insertAt = (str, sub, pos) => `${str.slice(0,pos)}${sub}${str.slice(pos)}`

    // price calcs
    if (getlength(ammount) > 3) {
        zeroes = ammount.slice(-3)
        mainDigits = ammount.slice(0,ammount.length-3)
        if (getlength(mainDigits) > 3) {
            if (mainDigits.slice(-3) === '000') {
                zeroes = 'MILLION'
                mainDigits = mainDigits.slice(0,mainDigits.length-3)
            }
            else if (mainDigits.slice(-2) === '00') {
                zeroes = 'MILLION'
                mainDigits = mainDigits.slice(0,mainDigits.length-2)
                mainDigits = insertAt(mainDigits, '.', mainDigits.length-1)
            }
            else if (mainDigits.slice(-1) === '0') {
                zeroes = 'MILLION'
                mainDigits = mainDigits.slice(0,mainDigits.length-1)
                mainDigits = insertAt(mainDigits, '.', mainDigits.length-2)
            }
            else{
                mainDigits = parseInt(mainDigits).toLocaleString('en-US')
            }
            // mainDigits = parseInt(mainDigits).toLocaleString('en-US')
        }
    }
    console.log(mainDigits);

</script>

<div class=" bg-light-200 dark:bg-dark-200 p-10 relative mx-auto w-full">
	<header class="my-8">
		<h3 class="text-3xl font-semibold text-center">{title}</h3>
	</header>
	<div class="text-center my-10">
		<div class="flex mx-auto w-fit">
            <span class="mb-auto dark:text-dark-400">UGX</span>
            <span class="font-bold text-7xl sm:text-8xl">{mainDigits}</span>
            <span class="my-auto ml-1 dark:text-dark-400">{zeroes}</span>
        </div>
	</div>
	<ol>
		<li class="flex gap-3 my-2"><Arrow/> Multipe file types</li>
		<li class="flex gap-3 my-2"><Arrow/> Multipe colors</li>
		<li class="flex gap-3 my-2"><Arrow/> Brand guidelines</li>
		<li class="flex gap-3 my-2"><Arrow/> Unlimited changes</li>
		<li class="flex gap-3 my-2"><Arrow/> Full ownership</li>
		<li class="flex gap-3 my-2"><Arrow/> Social media kit</li>
	</ol>
</div>

<style>
</style>
