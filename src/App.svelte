<script lang="ts">
	import { Carta, MarkdownEditor } from "carta-md";
	import "carta-md/default.css";

	const carta = new Carta({
		sanitizer: (html: string) => html,
		extensions: [],
	});

	let value = "";
</script>

<main>
	<MarkdownEditor {carta} bind:value />
</main>

<style>
</style>
