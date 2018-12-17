<template>
  <section>
    <sec-hero></sec-hero>
    <sec-about></sec-about>
    <sec-access></sec-access>
    <sec-sponsor :sponsors="sponsors"></sec-sponsor>
    <sec-staff></sec-staff>
    <sec-footer></sec-footer>
  </section>
</template>

<script>
  import secHero from '~/components/pages/Top/Hero.vue'
  import secAbout from '~/components/pages/Top/About.vue'
  import secAccess from '~/components/pages/Top/Access.vue'
  import secSponsor from '~/components/pages/Top/Sponsor.vue'
  import secStaff from '~/components/pages/Top/Staff.vue'
  import secFooter from '~/components/Footer.vue'

  export default {
    async asyncData({store}) {
      const [sponsors] = await Promise.all([
        store.dispatch("fetchSponsors")
      ])
      return {
        sponsors
      }
    },
    components: {
      secHero,
      secAbout,
      secAccess,
      secSponsor,
      secStaff,
      secFooter,
    },
  }
</script>

<style>

</style>
