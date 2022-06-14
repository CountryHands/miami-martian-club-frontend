<script>
	import promo1 from '../assets/videos/mm1.mp4';
</script>

<section class="h-screen flex flex-col justify-evenly items-center">
	<video class="w-11/12 lg:w-7/12 h-4/5" loop autoplay muted controls>
		<source src={promo1} type="video/mp4" />
	</video>
	<a
		href="home"
		class="flex place-items-center justify-center rounded bg-primary text-2xl text-white font-bold h-12 w-1/2 mt-2 shadow-lg shadow-white/50	
		transition transform hover:-translate-y-1 hover:scale-105 motion-reduce:transition-none motion-reduce:hover:transform-none"
		>JOIN THE CLUB</a
	>
</section>

