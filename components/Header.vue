<template lang="pug">
	header.header-wrapper
		.logo.py-2.px-4
			nuxt-link(to="/")
				v-avatar(color="grey lighten-2" size="44") MJ
		ul.navi-wrapper
			.navi
				a(href=`${process.env.SERVER}`) Node/Express Board
			.navi
				a(href=`${process.env.REACT}`) React/Next Board
</template>

<script>
export default {
	name: "Headers"
}
</script>

<style lang="scss" scoped>
.header-wrapper {
	background-color: #263238;
	color: $colorLighter;
  @include flex($SB, $CT);
	border-bottom: 1px solid $colorLighter;
	align-items: center;
	.logo {
		padding: 0 1.5em;
		color: #222;
  }
	.navi-wrapper {
    @include flex($SB, $CT);
		align-items: center;
		.navi {
			padding: 0.75em 1.5em;
    }
  }
}
</style>
