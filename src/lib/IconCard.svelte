<script>
	import githubIcon from './githubIcon.svg';
	import LinkedInIcon from './linkedinIcon.svg';
	import InstagramIcon from '$lib/instagramIcon.svg';
</script>

<div class="icon-card">
	<div class="img-card">
		<a target="_blank" rel="noreferrer" href="https://github.com/SikandarJODD">
			<img src={githubIcon} alt="stuff" />
		</a>
	</div>
	<div class="img-card">
		<a
			target="_blank"
			rel="noreferrer"
			href="https://www.linkedin.com/in/sikandar-bhide-911988211/"
		>
			<img src={LinkedInIcon} alt="github" />
		</a>
	</div>
	<div class="img-card">
		<a target="_blank" rel="noreferrer" href="https://www.instagram.com/sikandar.s.bhide/">
			<img src={InstagramIcon} alt="github" />
		</a>
	</div>
</div>

<style>
	.icon-card img {
		margin: 0px 3px;
		/* width: 25px; */
	}
	.icon-card {
		margin: 10px 0px;
		display: flex;
		align-items: center;
		justify-content: center;
		place-items: center;
	}
	.img-card {
		padding: 10px;
		margin: 0 4px;
		border-radius: 10px;
		transition: all 0.3s ease;
	}
	.img-card:hover {
		transition: all 0.3s ease;
		background: rgba(56, 103, 136, 0.724);
	}
	@media screen and (min-width: 501px) {
		img {
			width: 44px;
		}
	}
	@media screen and (max-width: 500px) {
		img {
			width: 38px;
			margin: 0;
		}
		.icon-card {
			margin: 4px 0;
		}
		.img-card {
			margin: 0;
		}
	}
</style>
