<template>
  <b-container class="p-4">
    <homenav />
    <b-row class="pt-3">
      <b-col cols="12">
        <b-card class="bg-none text-center border-0 animate__animated animate__fadeInUp">
          <b-img src="~/assets/img/barcamp-logo.png" fluid />
        </b-card>
        <b-card class="bg-none text-center text-white Roboto-light border-0 animate__animated animate__fadeInUp animate__delay-1.2s">
          <p class="d-none d-lg-block roboto-light" style="font-size:2.5em">
            <b class="roboto-fat" style="font-size:1.3em">{{ date }}</b> 2020 | {{ time }}
          </p>
          <p class="d-lg-none d-sm-block roboto-light" style="font-size:1.2em">
            <b class="roboto-fat" style="font-size:1.5em">{{ date }}</b> 2020
          </p>
          <p class="d-lg-none d-sm-block roboto-light" style="font-size:1.2em">
            {{ time }}
          </p>
          <countdown />
        </b-card>
      </b-col>
    </b-row>
    <b-row class="pt-2 pb-5 text-center animate__animated animate__fadeInUp animate__delay-1.3s">
      <b-col>
        <b-button
          href="https://forms.gle/bH4NuamofgKq4PXp9"
          target="_blank"
          variant="outline-light"
          size="md"
          class="p-3 mr-1"
          style="width:8.5em"
          pill
        >
          Be a Speaker
        </b-button>
        <b-button
          href="https://forms.gle/oUsnkzHNKjbNUPu88"
          target="_blank"
          variant="light"
          size="md"
          class="p-3 ml-1"
          style="width:8.5em; color:purple;"
          pill
        >
          Register Now
        </b-button>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
import Homenav from '~/components/home-nav'
import Countdown from '~/components/countdown'

export default {
  components: {
    Homenav,
    Countdown
  },
  data: () => {
    return {
      date: 'August 29',
      time: '1.30 to 7.20pm'
    }
  }
}
</script>
