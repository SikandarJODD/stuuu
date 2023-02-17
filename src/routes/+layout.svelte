<script>
	import { page } from '$app/stores';
	import Footer from './Footer.svelte';
	import './style.css';

	$: path = $page.route.id;
	let navs = [
		{
			title: '/',
			link: '/'
		},
		{
			title: 'Stufu',
			link: '/stuff'
		},
		{
			title: 'Fosto',
			link: '/fost'
		},
		{
			title: 'Phili',
			link: '/philli'
		}
	];
</script>

<main>
	<ul>
		{#each navs as tab}
			<li><a href={tab.link} class:active={path == tab.link}>{tab.title}</a></li>
		{/each}
	</ul>
	<slot />
	<Footer />
</main>

<style>
	ul > li {
		text-decoration: none;
		list-style: none;
		margin: 20px 10px 55px 10px;
	}
	ul {
		display: flex;
		justify-content: center;
		align-items: center;
	}
	ul > li > a {
		text-decoration: none;
		color: white;
		font-size: 1.5rem;
		padding: 10px 20px;
		/* border: 1px solid white; */
		border-radius: 30px;
		transition: all 0.3s ease;
	}
	ul > li > a:hover {
		/* background: #173756; */
		background: #173b5f;
		transition: all 0.3s ease;
	}
	.active {
		transition: all 0.3s ease;
		border: 1px solid rgb(42, 125, 248);
		background-color: #03142379;
	}
</style>
