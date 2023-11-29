<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppFumetti from './components/AppFumetti.vue'
import Store from './components/Store.vue'
import Misc from './components/Misc.vue'
import Contacts from './components/Contacts.vue'

export default {
	components: {
		AppHeader,
		AppJumbo,
		AppFumetti,
		Store,
		Misc,
		Contacts,
	}
}
</script>

<template>

	<AppHeader />
	<AppJumbo />
	<AppFumetti />
	<Store />
	<Misc />
	<Contacts />
		
</template>

<style scoped></style>
