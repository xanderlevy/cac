<script>
 import { Eye, EyeClosed } from "lucide-svelte";

	export let name;
	let checked = false;
</script>

<div style="display: flex; flex-direction: column;">
	<label
		for={name}
		style="border-bottom: 2px solid black; width: 100%; height: 100%;user-select: none; cursor: pointer;"
	>
		<p>
			{name}
			{#if checked}
				<Eye />
			{:else}
				<EyeClosed />
			{/if}
		</p>
	</label>
	<input style="display: none;" type="checkbox" bind:checked id={name} />
	{#if checked}
		<slot />
	{/if}
</div>

<style>
p{
margin: 5px;
display: flex;
justify-content: space-around;
}
</style>
