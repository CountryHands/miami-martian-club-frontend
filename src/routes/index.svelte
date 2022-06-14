<script>
	import HeaderMartian from '../components/headerMartian.svelte';
	import UniqueMartians from '../components/uniqueMartians.svelte';
	import MeetTheMartians from '../components/meetTheMartians.svelte';
	import Faq from '../components/faq.svelte';
	import RoadMap from '../components/roadMap.svelte';
	// import BuyMartian from '../components/buyMartian.svelte';
	import MartianDao from '../components/martianDao.svelte';
	import TeamMartians from "../components/team.svelte";
</script>

<HeaderMartian/>
<div class="mx-4 sm:container sm:mx-auto text-lg">
	<UniqueMartians />
	<MeetTheMartians/>
	<RoadMap />
	<Faq />
	<!-- <BuyMartian /> -->
	<MartianDao />
	<TeamMartians />
</div>

