<template>
    <div>
        <v-toolbar
        dark
        src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
        >
        <v-img
            alt="Vuetify Logo"
            class="shrink mr-2"
            contain
            src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
            transition="scale-transition"
            width="40"
        />

        <v-img
            alt="Vuetify Name"
            class="shrink mt-1 hidden-sm-and-down"
            contain
            min-width="100"
            src="https://cdn.vuetifyjs.com/images/logos/vuetify-name-dark.png"
            width="100"
        />
        <v-toolbar-title></v-toolbar-title>
        </v-toolbar>
    </div>
</template>

<script>
export default {
    name: "Toolbar"
}
</script>