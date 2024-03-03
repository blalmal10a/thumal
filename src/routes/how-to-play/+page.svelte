<svelte:head>
	<title>How to play Zodle</title>
	<meta name="description" content="How to play Zodle" />
</svelte:head>

<div class="text-column">
	<h1>How to play Zodle</h1>

	<p>
		Zodle hi <a href="https://www.nytimes.com/games/wordle/index.html">Wordle</a> clone a ni a, Thumal hawrawp nga (5) rin dik tur a ni. Entir nan a hnuai a mi ag khuan:
	</p>

	<div class="example">
		<span class="exact">t</span>
		<span class="exact">i</span>
		<span class="exact">l</span>
		<span class="close">t</span>
		<span class="missing">e</span>
	</div>

	<p>
		I rin zingah khian 

		<span class="exact">t</span>
		<span class="exact">i</span>
		<span class="exact">l</span>

		tihte khi i an awmna zawnah an awm dik thlap tihna a ni a,

a zawh leha 
		<span class="close">t</span>
		hi a thumalin a ken tel, mahse a awmna dik lo va awm tihna a ni a,
		<span class="missing">e</span>
		erawh hi chu a thumal rin dik turin a keng tel lo tihna a ni.
	</p>

	<div class="example">
		<span class="exact">t</span>
		<span class="exact">i</span>
		<span class="exact">l</span>
		<span class="exact">m</span>
		<span class="exact">u</span>
	</div>

	<p>vawi sarih (7) rin dikna hun i nei zel ang a.</p>
	<p>A chung a mi ang khian, a lo pawl vek a nih chuan i ring dik tihna a ni.</p>
</div>

<style>
	span {
		display: inline-flex;
		justify-content: center;
		align-items: center;
		font-size: 0.8em;
		width: 2.4em;
		height: 2.4em;
		background-color: white;
		box-sizing: border-box;
		border-radius: 2px;
		border-width: 2px;
		color: rgba(0, 0, 0, 0.7);
	}

	.missing {
		background: rgba(255, 255, 255, 0.5);
		color: rgba(0, 0, 0, 0.5);
	}

	.close {
		border-style: solid;
		border-color: var(--color-theme-2);
	}

	.exact {
		background: var(--color-theme-2);
		color: white;
	}

	.example {
		display: flex;
		justify-content: flex-start;
		margin: 1rem 0;
		gap: 0.2rem;
	}

	.example span {
		font-size: 1.4rem;
	}

	p span {
		position: relative;
		border-width: 1px;
		border-radius: 1px;
		font-size: 0.4em;
		transform: scale(2) translate(0, -10%);
		margin: 0 1em;
	}
</style>
