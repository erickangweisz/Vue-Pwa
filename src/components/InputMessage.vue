<template>
  <v-form>
    <v-container>
      <v-row>
        <v-col cols="12">
          
          <v-text-field
            v-model="message"
            outlined
            clearable
            label="message"
            type="text"
          >
            <template v-slot:append>
              <v-fade-transition leave-absolute>
                <v-progress-circular
                  v-if="loading"
                  size="24"
                  color="info"
                  indeterminate
                ></v-progress-circular>
                <img v-else width="24" height="24" src="https://cdn.vuetifyjs.com/images/logos/v-alt.svg" alt="">
              </v-fade-transition>
            </template>
          </v-text-field>

          <div class="text-center">
            <v-btn @click="clickMe" rounded color="primary" dark>Click me!</v-btn>
          </div>

        </v-col>
      </v-row>
    </v-container>
  </v-form>
</template>

<script>
export default {
    name: "InputMessage",

    data: () => ({
        message: '',
        loading: false
    }),

    methods: {
        clickMe () {
          this.loading = true
          this.message = 'Wait for it...'
          setTimeout(() => {
            this.loading = false
            this.message = 'You\'ve clicked me!'
          }, 2000)
        }
    }
}
</script>