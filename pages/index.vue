<template>
  <v-container
    :style="$vuetify.breakpoint.xl ? 'padding: 0 15%' : ''"
  >
    <v-row>
      <v-col
        cols="12"
        md="6"
        sm="12"
        class="d-flex flex-column justify-center"
      >
        <img
          src="@/assets/images/blob.svg"
        >
      </v-col>

      <v-col
        cols="12"
        md="4"
        sm="10"
        :class="$vuetify.breakpoint.xs ? 'd-flex flex-column justify-center align-center' : 'd-flex flex-column justify-center'"
      >
        <span>Hello!</span>
        <h1>I'm Julián</h1>
        <h2>Software Engineer</h2>
        <p>caca</p>
        <div>
          <v-btn
            dark
            x-large
            elevation="0"
            color="indigo"
            to="/contact"
            style="textTransform: none"
          >
            Contact me

            <img
              src="@/assets/icons/send-white.svg"
              height="18"
              width="18"
              class="mr-n1 ml-2"
            >
          </v-btn>
        </div>
      </v-col>

      <v-col
        cols="12"
        md="2"
        sm="2"
        :class="$vuetify.breakpoint.xs ? 'd-flex justify-center' : 'd-flex flex-column justify-center'"
      >
        <v-btn
          icon
          large
          fab
          color="indigo"
          href="https://www.linkedin.com/in/julián-de-pablo-torremocha"
          target="_blank"
        >
          <img
            src="@/assets/icons/linkedin.svg"
            height="28"
            width="28"
          >
        </v-btn>

        <v-btn 
          icon
          large
          fab
          color="indigo"
          href="https://github.com/julidpt"
          target="_blank"
        >
          <img
            src="@/assets/icons/github.svg"
            height="28"
            width="28"
          >
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<style lang="scss" scoped>
.container,
.row {
  height: 100%;
}

h1 {
  font-family: 'Poppins', sans-serif;
  font-size: 350%;
}
</style>

<script>
export default {
  head() {
    return {
      title: "Home",
    };
  },
};
</script>