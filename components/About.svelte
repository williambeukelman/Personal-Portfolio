<style>
  .btn {
    margin-top: -1.5rem;
    margin-bottom: 1.5rem;
  }
</style>

<script>
import { scale } from "svelte/transition";
let visible = false;
</script>

<input type="checkbox" class="btn-check" id="btn-check" bind:checked={visible}>
<label for="btn-check" class="btn btn-primary">
<h5>About Me</h5>
{#if visible}
	<div transition:scale>
		Lifelong interest in all things science, engineering, and computers.
    I am currently pursuing a degree in software development.
	</div>
{/if}
</label>

