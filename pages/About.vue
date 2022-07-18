<template>
  <div>
    <Banner :title="banner.title" :description="banner.description" />
    <div class="about section-space">
      <v-container>
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="about__heading">
              <h2 class="text-center mb-12 text-h4">
                About Katshi Way Design Creative
              </h2>
              <p>
                November 2013, six friends come together to discuss the
                possibility for a unique software company that doesn't pine to
                build product while producing solutions, that doesn't sell
                services while promising panaceas.
              </p>
              <p>
                Rather, we wanted to build a software company which addresses
                our shared core belief that
                <strong
                  >all companies are going to be software companies in one shape
                  or form by the end of the century</strong
                >.
              </p>
              <p>
                For us, there is an existential question every business is going
                to face in the coming decades: Are we going survive and lead
                with our own software? Or are we going to fail using the same as
                others or even none?
              </p>
              <p>
                We look to partner with owners, entrepreneurs and corporate
                businesses in answering that question; through their business
                domain knowledge, and our decades of software and business
                experience.
              </p>
              <p>
                Why Katshi Way Design Creative? We've called ourselves Katshi
                Way Design Creative (as have many others - we like company)
                because to deliver on our core belief, we knew we would need
                collaborators and colleagues who had mastered the Katshi Way
                Design Creative of software components from the network layer
                all the way up to the customer and the business need.
              </p>
              <p>
                With a team of Katshi Way Design Creative developers, we are
                able to help our clients run and grow great companies, using
                software built in partnership with us.
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
import Banner from '@/components/Banner'

export default {
  components: { Banner },
  layout: 'MainPageLayout',
  data() {
    return {
      banner: {
        title: 'About',
        description: `Katshi Way Design Creative is a software company providing data products and services designed to unlock business value, through
                the delivery of quality software.`,
      },
    }
  },
}
</script>

<style lang="scss" scoped>
.about {
  &-thumb {
    max-width: 77px;
    opacity: 0.5;
  }
  &__item {
    padding: 20px;
    &:hover {
      cursor: pointer;
      transition: all 0.5s ease-in;
      .about-thumb {
        transform: scale(1.2);
        transition: all 0.3s ease-in;
      }
    }
  }
}

.section-space {
  padding: 100px 50px;
}
</style>
