<template>
  <v-app-bar
        app
        color="white"
        flat
      >
        <v-container class="py-0 fill-height">
          <v-avatar
            class="mr-10"
            color="grey darken-1"
            size="32"
          >
            <span>GM</span>
          </v-avatar>

          <v-btn
            v-for="link in links"
            :key="link"
            text
          >
            {{ link }}
          </v-btn>

          <v-spacer></v-spacer>

          <v-responsive max-width="260">
            <v-text-field
              dense
              flat
              hide-details
              rounded
              solo-inverted
            ></v-text-field>
          </v-responsive>
        </v-container>
      </v-app-bar>
</template>

<script>
export default {
      data: () => ({
        links: [
          'Dashboard',
          'Messages',
          'Profile',
          'Updates',
        ],
      }),
    }
</script>

<style>

</style>
