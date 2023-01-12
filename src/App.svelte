<script lang="ts">
	import ModeSwitcher from './ModeSwitcher.svelte';
	import Tailwindcss from './Tailwindcss.svelte';
	let prompt = 'start typing here';
</script>
<Tailwindcss />
<ModeSwitcher />
<main class="p-4 text-center">
	<h1 class="text-7xl leading-normal  text-svelte">OpenAI frontend template!</h1>
	<p class="text-xl mt-12 mb-12">
		Unlock the Power of GPT-3 by creating a custom website to send prompts to the API.
	</p>

	<div class="prompt-container">
        <textarea bind:value={prompt} class="prompt-box text-black w-6/12 h-48 text-left align-top" />
    </div>

	<button class="bg-svelte dark:hover:bg-orange-800 hover:bg-orange-600 text-black dark:text-white hover:border-2 hover:border-black dark:hover:border-white font-bold py-2 px-4 rounded mt-6">
		Generate
	</button>
</main>