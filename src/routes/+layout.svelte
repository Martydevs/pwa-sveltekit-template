<script lang="ts">
  import { onMount } from 'svelte';
	import '../app.css';
  import { detectSWUpdate } from '$lib/utils/sw';
	let { children } = $props();

	onMount(() => {
		detectSWUpdate();
	})
</script>

{@render children()}
