<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import Store from './components/Store.vue'
import Misc from './components/Misc.vue'
import Contacts from './components/Contacts.vue'

export default {
	components: {
		AppHeader,
		AppMain,
		Store,
		Misc,
		Contacts,
	}
}
</script>

<template>

	<AppHeader />
	<AppMain />
	<Store />
	<Misc />
	<Contacts />
		
</template>

<style scoped></style>
