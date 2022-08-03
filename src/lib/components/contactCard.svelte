<script>
    export let icon = 'fab fa-facebook'
    export let text = '@amaritslab'
    export let text2 = ''
</script>

<div class="p-8 xl:p-20 dark:hover:bg-white dark:bg-slate-900 bg-slate-300 hover:bg-black aspect-square flex flex-col justify-center text-center transition-all duration-700 ">
    <i class="{icon} text-8xl text-slate-500 mb-6"></i>
    <span class=" dark:text-slate-500">{text}</span>
    {#if text2}
    <span class=" dark:text-slate-500">{text2}</span>
    {/if}
</div>

<style>
    div{
        border-radius: 1.5rem;
    }
    div:hover span{
        @apply dark:text-slate-900 text-slate-100
    }
</style>