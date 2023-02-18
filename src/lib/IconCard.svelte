<script>
	import githubIcon from './githubIcon.svg';
	import LinkedInIcon from './linkedinIcon.svg';
	import InstagramIcon from './instagramIcon.svg';
</script>

<div class="icon-card">
	<div class="img-card">
		<a target="_blank" rel="noreferrer" href="https://github.com/SikandarJODD">
			<img src={githubIcon} alt="github" />
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
		/* padding: 20px; */
	}
	.icon-card {
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
		/* background: rgba(56, 103, 136, 0.724); */
	}
	@media screen and (min-width: 700px) and (max-width: 1300px) {
		img {
			width: 30px;
		}
	}
</style>
