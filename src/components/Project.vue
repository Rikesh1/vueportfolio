<template>
	<div class="projects">
		<div class="item" :key="project.id" v-for="project in projects">
			<a :href="project.link" target="_blank">
				<img :src="project.image" :alt="project.title">
			</a>
			<a :href="project.link" target="_blank" class="btn-light">
				<font-awesome-icon :icon="['fas', 'eye']" /> Project
			</a>
			<a :href="project.githubLink" target="_blank" class="btn-dark">
				<font-awesome-icon :icon="['fab', 'github']" /> Github
			</a>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Project',
		props: ['projects']
	}
</script>