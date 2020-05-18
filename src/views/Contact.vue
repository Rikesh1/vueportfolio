<template>
	<div>
		<main id="contact">
			<h1 class="lg-heading">
				Contact 
				<span class="text-secondary"> Me</span>
			</h1>
			<h2 class="sm-heading">
				This is how you can reach me...
			</h2>
			<div class="boxes">
				<div>
					<span class="text-secondary"><font-awesome-icon :icon="['fas', 'envelope']" /> Email:</span> rmaharjan74@gmail.com
				</div>
				<div>
					<span class="text-secondary"><font-awesome-icon :icon="['fas', 'phone']" /> Phone:</span> (+977) 9808963778
				</div>
				<div>
					<span class="text-secondary"><font-awesome-icon :icon="['fas', 'map-marker-alt']" /> Address:</span> Chyasal Lalitpur Bagmati Nepal
				</div>
			</div>
		</main>

		<Footer />
	</div>
</template>

<script>
	import Footer from '@/components/layouts/Footer.vue'

	export default {
		name: 'Contact',
		components: {
			Footer
		}
	}
</script>