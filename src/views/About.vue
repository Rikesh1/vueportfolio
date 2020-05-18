<template>
	<div>
		<main id="about">
			<h1 class="lg-heading">
				About 
				<span class="text-secondary"> Me</span>
			</h1>
			<h2 class="sm-heading">
				Let Me Tell You A Few Things...
			</h2>
			<div class="about-info">
				<img src="../assets/img/portrait.jpg" alt="Rikesh Maharjan" class="bio-image">

				<div class="bio">
					<h3 class="text-secondary">BIO</h3>
					<p>I am passionate, hardworking and enthusiastic web developer. My interest on coding increases when i first completed a small application to make calculator in my college. From that day, I know I can be a good web developer.</p>
				</div>

				<div v-for="experience in experiences" :key="experience.id" :class="`job job-${experience.id}`">
					<h3>{{ experience.company }}</h3>
					<h6>{{ experience.position }}</h6>
					<p>{{ experience.description }}</p>
				</div>
			</div>
		</main>
		
		<Footer />
	</div>
</template>

<script>
	import Footer from '@/components/layouts/Footer.vue'

	export default {
		components: {
			Footer
		},
		data() {
			return {
				experiences: [
					{
						id: 1,
						company: 'Nextnepal IT Solutions',
						position: 'Backend Developer',
						description: 'I first started my career from a small start up company at Nextnepal IT Solutions as a junior laravel developer. I worked there for two years and six months and learned lots of new skills and gain knowledge of IT organization.'
					},
					{
						id: 2,
						company: 'Freelancing',
						position: 'Full Stack Developer',
						description: 'During my career, I have also done some freelancing projects. I put out all my skills and knowledge that I gained from my official job into these projects which help me finished these projects at right time.'
					},
					{
						id: 3,
						company: 'College Projects',
						position: 'Programmer',
						description: 'I have also done some college projects during my academic period where I learned the basic and practical skills of web development. These skills helped me later in my career.'
					}
				]
			}
		}
	}
</script>