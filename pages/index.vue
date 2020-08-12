<template>
  <main>
    <Herobox />
    <FeaturesSection />
    <Cards />
    <Timeline />
    <Pricing />
  </main>
</template>

<script>
import Herobox from '@/components/Herobox'
import FeaturesSection from '@/components/FeaturesSection'
import Cards from '@/components/Cards'
import Timeline from '@/components/Timeline'
import Pricing from '@/components/Pricing'

export default {
  components: {
    Herobox,
    FeaturesSection,
    Cards,
    Timeline,
    Pricing,
  },
}
</script>

<style></style>
