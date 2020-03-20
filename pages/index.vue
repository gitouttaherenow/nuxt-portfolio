<template>
<div>
	<HomeHero />
	<HomeAbout />
	<HomeProjects />
	<Contact />
</div>
</template>

<script>

import HomeHero from '@/components/HomeHero';
import HomeAbout from '@/components/HomeAbout';
import HomeProjects from '@/components/HomeProjects';
import Contact from '@/components/Contact';

export default {
	name: 'home',
	components: {
		HomeHero,
		HomeAbout,
		HomeProjects,
		Contact
	}
}
</script>