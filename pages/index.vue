<template>
  <div>
    <!-- Hero Start -->
    <Hero />
    <!-- Hero End -->

    <!-- Features Start -->
    <section class="py-20 bg-gray-50 shadow-inner">
      <div class="px-4 mx-auto text-center max-w-7xl sm:px-6 lg:px-8">
        <h2 class="text-3xl font-bold tracking-tight text-accent sm:text-4xl md:text-5xl xl:text-6xl">
          Citizen centric services
        </h2>
        <p class="max-w-md mx-auto mt-3 text-base text-gray-500 sm:text-lg md:mt-5 md:text-xl md:max-w-3xl">
          We make daily waste collection and transport easy and transparent
        </p>
      </div>

      <div class="container max-w-6xl mx-auto">
        <div class="grid grid-cols-4 gap-8 mt-10 sm:grid-cols-4 lg:grid-cols-12 sm:px-8 xl:px-0">
          <div class="relative flex flex-col items-center justify-start col-span-4 px-8 py-12 space-y-4 overflow-hidden">
            <div class="p-3 text-white bg-primary shadow-primary rounded-full">
              <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
              </svg>
            </div>
            <h4 class="text-xl font-medium text-accent">
              Upcycle Economy Model
            </h4>
            <p class="text-base text-center text-gray-500">
              We reuse waste material and create new products and try to give back to nature things which can be reused also later.
            </p>
          </div>

          <div class="relative flex flex-col items-center justify-start col-span-4 px-8 py-12 space-y-4 overflow-hidden">
            <div class="p-3 text-white bg-primary shadow-primary rounded-full">
              <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
              </svg>
            </div>
            <h4 class="text-xl font-medium text-accent">
             Blockchain based Supply Chain
            </h4>
            <p class="text-base text-center text-gray-500">
              Smart contracts are used to track end-point and terminal of Etheretum based waste supply chain
            </p>
          </div>

          <div class="relative flex flex-col items-center justify-start col-span-4 px-8 py-12 space-y-4 overflow-hidden">
            <div class="p-3 text-white bg-primary shadow-primary rounded-full">
              <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
              </svg>
            </div>
            <h4 class="text-xl font-medium text-accent">
              Urban Management Made Easy
            </h4>
            <p class="text-base text-center text-gray-500">
              Citizen planners are capable of visualzing Waste data, such as track records of waste collection, delivery.
            </p>
          </div>
        </div>
      </div>
    </section>
    <!-- Features End -->

    <!-- Testimonials Start-->
    <Testimonials :testimonials="testimonials"/>
    <!-- Testimonials End-->

    <!-- Call To Action Start -->
    <CallAction />
    <!-- Call To Action End -->
  </div>
</template>

<script>
import Hero from '~/components/Hero.vue';
import Testimonials from '~/components/Testimonials.vue';
import CallAction from '~/components/CallAction.vue';

export default {
  components: {
    Hero,
    Testimonials,
    CallAction
  },
  head: {
    title: 'ReuseChain - Blockchain and Upcycle for Waste',
    meta: [ // SEO Tags
      {
        hid: 'description',
        name: 'description',
        content: 'Blockchain and Upcyle Economy in Smart City Waste Management'
      }
    ]
  },
  data: () => ({
    testimonials: [
      {
        id: 1,
        name: 'Katerina Federova ',
        jobTitle: 'Urban Planner',
        message: 'We were having trouble in manaing our large city with less manpower. Hopefully we find a solution now '
      },
      {
        id: 2,
        name: 'Zuana Margerta',
        jobTitle: 'Citizen',
        message: 'We are now capable of tracking the incoming and ongoing waste trucks'
      },
      {
        id: 3,
        name: 'Viltatova Mihaolova',
        jobTitle: 'Data Scientist.',
        message: 'We thought we are running out of idea . Now blockchain solves it! great'
      }
    ]
  })
}
</script>
