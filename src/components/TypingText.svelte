<script lang="ts">
	import { onMount } from 'svelte';

	export let text: string;
	export let classList: string = '';
	export let latency: number = 0;
	export let caret: boolean = true;
    export let speed: number = 80
	let visibleText = '';
	let isCaret = true;

	async function showText() {
		while (text.length) {
			let time = Math.floor(Math.random() * speed);
			await new Promise((res) => setTimeout(() => res(1), time));
			visibleText += text.slice(0, 1);
			text = text.slice(1, text.length);
		}

		if (!caret) isCaret = false;
	}
	onMount(() => {
		isCaret = false;
		setTimeout(() => {
			isCaret = true;
			showText();
		}, latency);
	});
</script>

<div class="z-10">
	<span class={classList}>{visibleText}</span>
	{#if isCaret}
		<span class={`${classList} absolute caret rubik-mono`}>|</span>
	{/if}
</div>

<style lang="sass">
    @import url('https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300..900;1,300..900&display=swap')
    .caret
        display: inline
        animation: splash 0.7s infinite
        transform: translate(2px, -1px)

    .rubik-mono
        font-family: "Rubik", sans-serif
        font-optical-sizing: auto
        font-weight: 400
        font-style: normal

    @keyframes splash 
        from 
            opacity: 1

        50%
            opacity: 0
        
        to 
            opacity: 1
            

</style>
