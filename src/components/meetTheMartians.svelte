<script>
	import martian8 from '../assets/images/8.png';
	import martian35 from '../assets/images/35.png';
	import martian66 from '../assets/images/66.png';
	import martian312 from '../assets/images/312.png';
	import martian14 from '../assets/images/14.png';
	import martian53 from '../assets/images/53.png';
	import martian174 from '../assets/images/174.png';
	import martian203 from '../assets/images/203.png';
	import martian1873 from '../assets/images/1873.png';
	import martian573 from '../assets/images/573.png';
	import martian492 from '../assets/images/492.png';
	import martian577 from '../assets/images/577.png';

	let martianImages = [
		martian8,
		martian35,
		martian66,
		martian312,
		martian14,
		martian53,
		martian174,
		martian203,
		martian1873,
		martian573,
		martian492,
		martian577
	];

	$: setInterval(nextSlide, 300);

	const nextSlide = () => {
		const tempArray = [...martianImages];
		if (tempArray.length > 0) {
			const e = tempArray.shift();
			if (e) {
				tempArray.push(e);
				martianImages = tempArray;
			}
		}
	};
</script>

<section id="meetTheMartians" class="h-full place-content-center text-white my-32">
	<h1 class="text-6xl text-primary font-black my-8">
		Meet <span class="text-white">The</span> Miami <span class="text-white">Martians</span>
	</h1>
	<div class="h-full flex place-content-center">
		<img 
        src={martianImages[0]} 
        alt="A Miami Martian"
        class="sm:w-10/12" />
	</div>
</section>
