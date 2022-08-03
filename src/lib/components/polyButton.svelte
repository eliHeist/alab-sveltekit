<script>
    import {goto} from '$app/navigation';

    export let link;
    export let text = 'Text';
    export let cls = ''

    const Go = () => {
        goto(link)
    } 
</script>

<button on:click={Go} class="{cls} bg-black dark:bg-white dark:text-black text-white hover:text-primary-900 text-2xl relative py-4 px-10 hover:bg-primary-900 hover:dark:bg-primary-900 before:dark:bg-white before:bg-black ">
    <span>{text}</span><i></i>
</button>

<style>
    /* From uiverse.io by @mrhyddenn */
button {
  text-transform: uppercase;
  letter-spacing: 0.1em;
  transition: 0.5s;
  border: none;
}
button.primary{
  @apply bg-primary-900 text-white hover:text-white hover:bg-slate-900 
}

button::before {
  content: '';
  position: absolute;
  inset: 2px;
}
button.primary:before{
  @apply bg-primary-900
}

button span {
  position: relative;
  z-index: 1;
}

button i {
  position: absolute;
  inset: 0;
  display: block;
}

button i::before {
  content: '';
  width: 10px;
  height: 6px;
  top: -3.5px;
  left: 80%;
  transform: translateX(-50%);
  transition: 0.5s;
  @apply absolute bg-slate-900 border-2 border-solid border-primary-900
}
button.primary i::before{
  @apply border-slate-900 dark:border-white bg-primary-900
}

button:hover i::before {
  width: 20px;
  left: 20%;
}

button i::after {
  content: '';
  position: absolute;
  width: 10px;
  height: 6px;
  bottom: -3.5px;
  left: 20%;
  transform: translateX(-50%);
  transition: 0.5s;
  @apply bg-slate-900 absolute border-2 border-solid border-primary-900
}
button.primary i::after{
  @apply border-slate-900 dark:border-white bg-primary-900
}

button:hover i::after {
  width: 20px;
  left: 80%;
}
</style>