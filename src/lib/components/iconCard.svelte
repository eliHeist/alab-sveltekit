<script>
    export let title = "collaborative design";
    export let icon = "i";
    export let i_color = '#fff';
</script>

<div class="">
    <div class="grid bg-white place-center" style="background-color: {i_color};">
        <i class="{icon}"></i>
    </div>
    <h2 class="">
        {title}
    </h2>
    <p class="">
        <slot>No text to display!</slot>
    </p>
</div>

<style>

</style>
