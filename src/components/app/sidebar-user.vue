<template functional lang="pug">
	.user-panel(v-if="props.user")
		.info {{ props.user.name || props.user.email }}
		!=' '
		a.logout-button(@click="parent.logout()"): i.fas.fa-sign-out-alt
</template>