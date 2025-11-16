<script lang="ts">
	import { getFoo } from './test.remote.js';
</script>
<svelte:boundary>
	{@const foo = await getFoo()}
	<p>Everything here is doubled</p>
	<button class="border" onclick={() => console.log("I'm clickable")}>
		Click me and check log
	</button>
</svelte:boundary>