<script>
	import FloatingArea from './floatingArea.svelte';
	import FloatingInput from './floatingInput.svelte';
</script>

<form method="post">
    <div class="mb-8">
        <FloatingInput label='Name' name='full_name' type='text'/>
    </div>
    <div class="grid grid-cols-2 gap-4">
        <FloatingInput label='Email' name='email' type='email'/>
        <FloatingInput label='Phone' name='phone' type='tel'/>
    </div>
    <div class="my-8">
        <FloatingArea label='Message' name='message' type='text'/>
    </div>
    <div class="mt-8">
        <button type="submit" class=" bg-primary-900 py-4 px-8 hover:bg-primary-500 font-semibold text-xl"><i class="fas fa-send mr-3"></i>Send</button>
    </div>
</form>

<style>
    button{
        border-radius: 1.2rem;
    }
</style>