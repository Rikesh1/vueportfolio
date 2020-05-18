<template>
	<header>
		<div class="menu-btn" :class="{'close': showMenu}" @click="toggleMenu">
			<div class="btn-line"></div>
			<div class="btn-line"></div>
			<div class="btn-line"></div>
		</div>

		<nav class="menu" :class="{'show': showMenu}">
			<div class="menu-branding" :class="{'show': showMenu}">
				<div class="portrait"></div>
			</div>
			<ul class="menu-nav" :class="{'show': showMenu}">
				<li class="nav-item" :class="{'show': showMenu}">
					<router-link to="/" class="nav-link" exact active-class="current" @click.native="toggleMenu">
						Home
					</router-link>
				</li>
				<li class="nav-item" :class="{'show': showMenu}">
					<router-link to="/about" class="nav-link" active-class="current" @click.native="toggleMenu">
						About Me
					</router-link>
				</li>
				<li class="nav-item" :class="{'show': showMenu}">
					<router-link to="/work" class="nav-link" active-class="current" @click.native="toggleMenu">
						My Portfolio
					</router-link>
				</li>
				<li class="nav-item" :class="{'show': showMenu}">
					<router-link to="/contact" class="nav-link" active-class="current" @click.native="toggleMenu">
						How To Reach Me
					</router-link>
				</li>
			</ul>
		</nav>
	</header>
</template>

<script>
	export default {
		name: "Header",
		data() {
			return {
				showMenu: false
			}
		},
		methods: {
			toggleMenu() {
				if (!this.showMenu) {
					this.showMenu = !this.showMenu;
				}
				else {
					this.showMenu = !this.showMenu;
				}
			}
		}
	}
</script>