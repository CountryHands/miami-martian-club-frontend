<script>
	import devMartian from '../assets/images/country.png';
    import nibu from '../assets/images/nibu.jpeg';
    import nick from '../assets/images/nick.png';
    import richie from '../assets/images/richie.png';
    import soyMartian from '../assets/images/soy_martian.png';
    import mike from '../assets/images/mike.png';
    import terry from '../assets/images/terry.png';
    import wolfie from '../assets/images/wolfie.png';


	let teamMembers = [
		{
			name: 'PartyMike',
			title: 'CEO and Founder',
			image: mike
		},
        {
			name: 'Nibu',
			title: 'COO',
			image: nibu
		},
        {
			name: 'CousinTerry',
			title: 'Community Engagement',
			image: terry
		},
        {
			name: 'CountryHands',
			title: 'The Dev',
			image: devMartian
		},
        {
			name: 'Nick',
			title: 'Wiz',
			image: nick
		},
        {
			name: 'WolfieWax',
			title: 'Acquisitions',
			image: wolfie
		},
        {
			name: 'RichieRich',
			title: 'Magic Maker',
			image: richie
		},
        {
			name: 'Soy',
			title: 'Community Manager',
			image: soyMartian
		},

	];
</script>

<section id="teamMartians" class="h-full place-content-center text-white my-32">
	<h1 class="text-6xl text-primary font-black my-8">
		<span class="text-shadow">Meet</span>
		<span class="text-white">The</span>
		<span class="text-shadow">Team</span>
	</h1>
	<div class="h-full grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-10 sm:gap-8 lg:gap-10">
		{#each teamMembers as teamMember}
			<div class="flex flex-col">
				<img src={teamMember.image} alt="A Miami Martian Team Member" class="rounded-lg" />
				<div class="flex flex-col mt-4 justify-between items-center">
					<p class="font-bold">@{teamMember.name}</p>
					<p class="flex place-items-center justify-center rounded bg-secondary text-black font-bold w-10/12 mt-2">{teamMember.title}</p>
				</div>
			</div>
		{/each}
	</div>
</section>

<style>
	.text-shadow {
		text-shadow: 1px 0 20px rgb(200 255 0 / 31%);
	}
</style>
