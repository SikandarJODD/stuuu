<!-- this consist of All types of Images including 
    .all .mobile .small .large .medium
    .mobile for mobile view
    .small for small view
    .medium for medium view
    .large for large view
    small + large == mdeium + medium 
    Size : 600px -> small : 200px and large : 400px
    medium : 300px * 2

    remember Footer is on positon not fixed stuff
 -->
<script>
	import img1large from './img1large.jpeg';
	import img2large from './img2large.jpeg';
	import img4large from './img4large.jpg';
	import img5large from './img5large.jpg';
	import img6large from './img6large.jpg';
	import img7large from './img7large.jpg';
	import img8large from './img8large.jpg';
	import img9large from './img9large.jpg';
	import img10large from './img10large.jpg';

	import img1medium from './img1medium.jpg';
	import img2medium from './img2medium.jpg';
	import img3medium from './img3medium.jpg';
	import img4medium from './img4medium.jpg';
	import img5medium from './img5medium.jpg';
	import img6medium from './img6medium.jpg';
	import img7medium from './img7medium.png';
	import img8medium from './img8medium.jpg';
	import img9medium from './img9medium.jpg';
	import img10medium from './img10medium.jpg';
	import img11medium from './img11medium.jpg';
	import img12medium from './img12medium.jpg';
	import img13medium from './img13medium.jpg';
</script>

<main>
	<h1>Aesthetic Vibes</h1>
	<div class="row">
		<div class="column">
			<img src={img2medium} class="all mobile medium" alt="aesthetic" />
			<img src={img6large} class="all mobile large" alt="aesthetic" />
			<img src={img3medium} class="all mobile medium" alt="aesthetic" />
		</div>
		<div class="column">
			<img src={img4large} class="all mobile large" alt="aesthetic" />
			<img src={img5medium} class="all mobile medium" alt="aesthetic" />
			<img src={img12medium} class="all mobile medium" alt="aesthetic" />
		</div>
		<div class="column">
			<img src={img1medium} class="all mobile medium" alt="aesthetic" />
			<img src={img1large} class="all mobile large" alt="aesthetic" />
			<img src={img9medium} class="all mobile medium" alt="aesthetic" />
		</div>
		<!-- <div class="column">
			<img src={img4medium} class="all mobile medium" alt="aesthetic" />
			<img src={img13medium} class="all mobile medium" alt="aesthetic" />
			<img src={img5large} class="all mobile large" alt="aesthetic" />
		</div>
		<div class="column">
			<img src={img7medium} class="all mobile medium" alt="aesthetic" />
			<img src={img7large} class="all mobile large" alt="aesthetic" />
			<img src={img11medium} class="all mobile medium" alt="aesthetic" />
		</div>
		<div class="column">
			<img src={img8medium} class="all mobile medium" alt="aesthetic" />
			<img src={img1medium} class="all mobile medium" alt="aesthetic" />
			<img src={img8large} class="all mobile large" alt="aesthetic" />
		</div> -->
	</div>
</main>

<style>
	h1 {
		margin-top: 20px;
		font-size: 3.5rem;
		text-align: center;
	}

	.all {
		border-radius: 40px;
	}
	.medium {
		width: 320px;
		height: 350px;
	}
	.large {
		width: 320px;
		height: 520px;
	}

	.row {
		margin-top: 20px;
		display: -ms-flexbox; /* IE10 */
		display: flex;
		-ms-flex-wrap: wrap; /* IE10 */
		flex-wrap: wrap;
		padding: 0 3%;
		justify-content: center;
	}
	/* Create four equal columns that sits next to each other */
	.column {
		max-width: 26%;
		padding: 0 4px;
	}
	.column img {
		margin: 10px 0px;
		/* vertical-align: middle; */
		/* width: 100%; */
	}
	/* Responsive layout - makes a two column-layout instead of four columns */
	/* @media screen and (max-width: 800px) {
		.column {
			-ms-flex: 50%;
			flex: 50%;
			max-width: 50%;
		}
		.row {
			padding: 0;
		}
		img {
			margin: 10px;
		}
	} */

	/* Responsive layout - makes the two columns stack on top of each other instead of next to each other */
	@media screen and (max-width: 600px) {
		h1 {
			margin-top: 0px;
			font-size: 2.4rem;
			text-align: center;
		}
		.row {
			display: flex;
			flex-wrap: wrap;
			justify-content: center;
			align-items: center;
		}
		.column {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			-ms-flex: 100%;
			flex: 100%;
			max-width: 100%;
		}
		.medium {
			width: 310px;
			height: 300px;
		}
		.large {
			width: 310px;
			height: 490px;
		}
	}
	@media screen and (min-width: 900px) and (max-width: 1290px) {
		.row {
			display: flex;
			flex-wrap: wrap;
			justify-content: center;
		}
		/* Create four equal columns that sits next to each other */
		.column {
			max-width: 32%;
		}
		.column img {
			width: 100%;
			vertical-align: middle;
		}
		.all {
			border-radius: 20px;
		}
		.medium {
			width: 280px;
			height: 320px;
		}
		.large {
			width: 300px;
			height: 430px;
		}
	}
</style>
