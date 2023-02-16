<script>
	import imgMain from './main.jpg';
	import SmallCard from './SmallCard.svelte';
</script>

<div class="container">
	<div class="card">
		<h1>Welcome to Fili - Phili</h1>
		<h2>Sikandar.S.Bhide</h2>
		<div class="active">
			<SmallCard />
		</div>
	</div>

	<div class="img-card">
		<img src={imgMain} alt="Anime" />
	</div>
</div>

<style>
	.container {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		margin: 10px 0;
	}
	.img-card img {
		width: 380px;
		height: 500px;
		border-radius: 40px;
		position: relative;
		bottom: 20px;
		box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
		transition: all 0.3s ease;
	}
	.img-card > img:hover {
		transition: all 0.3s ease;
		transform: scale(1.04);
	}
	h1 {
		margin: 10px 0;
		font-size: 2.9rem;
		color: rgba(100, 234, 252, 0.889);
	}
	h2 {
		color: rgb(210, 219, 232);
		font-family: monospace;
		font-size: 1.3rem;
	}
	@media (min-width: 320px) {
		/* smartphones, iPhone, portrait 480x320 phones */
		h1 {
			font-size: 2.3rem;
		}
		.container {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
		}
		.img-card img {
			width: 270px;
			height: 370px;
			bottom: 0;
			margin: 30px 0;
		}
		.active {
			display: none;
		}
	}
</style>
