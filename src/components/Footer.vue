<template>
  <v-footer dark padless>
    <v-card
      flat
      tile
      class="black white--text py-5 px-5 text-center"
      width="100%"
    >
      <v-row>
        <v-col cols="12" sm="4">
          <v-card-text class="white--text pt-2">
            <img src="../assets/nmLogoWhite.png" class="logo" />
          </v-card-text> 
        </v-col>

        <v-col cols="12" sm="4">
          <v-card-text class="pt-2">
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-1 white--text"
              icon
            >
              <v-icon size="24px">
                {{ icon }}
              </v-icon>
            </v-btn>
            <br/>
            <span> © 2022 NM, Inc. </span>&nbsp;
          </v-card-text>
        </v-col>
        <v-col cols="12" sm="4">
          <v-card-text class="pt-2 mt-4">
            Created by Nyembo Morisho
          </v-card-text>
        </v-col>
      </v-row>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    icons: [
      "mdi-facebook", "mdi-twitter", "mdi-instagram", "mdi-linkedin"
    ]
  })
};
</script>

<style>
.logo {
  width: 60px;
  height: 40px;
}
</style>