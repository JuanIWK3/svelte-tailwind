<div class="container-outer">
	<div class="container-inner">
		<div class="card z-10">
			<div class="card-body">
				<div class="card-title text-4xl font-bold">
					<h1 class="title">Serviços</h1>
				</div>
				<ul>
					<li>Manutenção</li>
					<li>Instalação</li>
					<li>Limpeza</li>
					<li>Reparo</li>
				</ul>
			</div>
		</div>
	</div>
	<div class="container-inner bg-base-200">
		<div class="card">
			<div class="card-body">
				<div class="card-title text-4xl font-bold">
					<h1 class="title">Produtos</h1>
				</div>
				<ul>
					<li>Mousepad</li>
					<li>Headset</li>
					<li>Monitor</li>
					<li>Teclado</li>
					<li>Mouse</li>
				</ul>
			</div>
		</div>
	</div>
</div>

<style lang="postcss">
	:global(html) {
		background-color: theme(colors.gray.100);
	}

	.container-outer {
		@apply flex flex-col h-screen sm:flex-row;
	}

	.container-inner {
		@apply flex flex-col items-center justify-center h-screen w-full cursor-pointer transition-all text-center;
		@apply hover:h-[110%] sm:hover:w-[110%] sm:hover:h-screen;
	}
	.card {
		@apply transition-all duration-200;
	}
	.container-inner:hover .card {
		@apply scale-105;
	}
</style>
