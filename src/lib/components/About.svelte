<script lang="ts">
	const cards = [
		{
			tag: 'what_i_do',
			body: 'Build simple, fast software. Then rethink and ponder the foundations everything stands on — is it bedrock, or just beach sand.',
			className: 'text-syn-green'
		},
		{
			tag: 'how_i_work',
			body: 'Blank sheet of paper. Dumb, simple systems. Complexity is my sworn enemy and I am at war with it daily.',
			className: 'text-syn-cyan'
		},
		{
			tag: "where_i'm_headed",
			body: 'Who knows. Not me. The world is uncertain and so am I — currently heading wherever the wind sorts me.',
			className: 'text-syn-purple'
		}
	];
</script>

<section id="about" class="border-t border-line bg-panel py-20">
	<div class="mx-auto max-w-6xl px-6">
		<h2 class="text-sm text-muted">
			<span class="text-syn-cyan">01</span> // about
		</h2>
		<p class="mt-4 max-w-2xl text-3xl font-semibold tracking-tight text-fg sm:text-4xl">
			Turning ideas into clean, somewhat working code.
		</p>

		<div class="mt-10 grid gap-5 md:grid-cols-3">
			{#each cards as card (card.tag)}
				<article class="rounded border border-line bg-bg p-6">
					<h3 class="text-sm font-semibold {card.className}">{card.tag}</h3>
					<div class="mt-3 h-px w-full bg-line-strong"></div>
					<p class="mt-4 text-sm leading-relaxed text-muted">{card.body}</p>
				</article>
			{/each}
		</div>
	</div>
</section>
