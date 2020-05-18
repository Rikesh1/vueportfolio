<template>
	<div>
		<main id="work">
			<h1 class="lg-heading">
				My 
				<span class="text-secondary"> Work</span>
			</h1>
			<h2 class="sm-heading">
				Check out some of my projects...
			</h2>
			<Project :projects="projects" />
		</main>
		
		<Footer />
	</div>
</template>

<script>
	import Footer from '@/components/layouts/Footer.vue'
	import Project from '@/components/Project.vue'

	export default {
		components: {
			Project,
			Footer
		},
		data() {
			return {
				projects: [
					{
						id: 1,
						title: 'Sann International College',
						image: require('../assets/img/projects/sann.png'),
						link: 'http://www.sann.edu.np',
						githubLink: '#'
					},
					{
						id: 2,
						title: 'Infranepal',
						image: require('../assets/img/projects/infranepal.png'),
						link: 'http://www.infranepal.com',
						githubLink: '#'
					},
					{
						id: 3,
						title: 'Dreamnepal',
						image: require('../assets/img/projects/dreamnepal.png'),
						link: 'http://www.dreamnepal.com.np',
						githubLink: '#'
					},
					{
						id: 4,
						title: 'Global Visa Advisor Consultancy',
						image: require('../assets/img/projects/globalvisaadvisor.png'),
						link: 'http://www.globalvisaadvisor.com',
						githubLink: '#'
					},
					{
						id: 5,
						title: 'Kinumna',
						image: require('../assets/img/projects/kinumna.png'),
						link: 'https://www.kinumna.com',
						githubLink: '#'
					},
					{
						id: 6,
						title: 'Sasto Outlet',
						image: require('../assets/img/projects/sastooutlet.png'),
						link: 'https://www.sastooutlet.com',
						githubLink: '#'
					}
				]
			}
		}
	}
</script>