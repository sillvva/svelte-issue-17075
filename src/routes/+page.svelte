<svelte:boundary>
	{@const foo = await 1}
	<p>Everything here is doubled</p>
	<button class="border" onclick={() => console.log("I'm clickable")}>
		Click me and check log
	</button>
</svelte:boundary>