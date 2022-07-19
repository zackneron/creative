<template>
  <div>
    <div class="hero">
      <v-container class="lg-container">
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="hero__content text-center">
              <h1 class="mb-4 text-h3">Katshi Way Design Creative</h1>
              <p class="text-h6 font-weight-light">
                Welcome to <strong>Katshi Way Design Creative</strong>. We are a
                software company. We believe in unlocking business value through
                the delivery of measurable
                <strong>high quality products and solutions</strong>.
              </p>
              <small
                >We are a proud to offer excellent service in Africa since
                2013.</small
              >
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="about section-space">
      <v-container class="">
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="about__heading text-center">
              <h2 class="mb-6 text-h4">About Us</h2>
              <p class="text-h5 font-weight-light">
                We provide software products and services and this is how we
                work:
              </p>
            </div>
          </v-col>
        </v-row>
        <v-row justify="center" align="center">
          <v-col
            v-for="items in aboutItems"
            :key="items.icon"
            cols="12"
            sm="6"
            md="4"
          >
            <div class="about__item text-center">
              <img
                class="about-thumb"
                :src="items.icon"
                alt="Analysis & Operations"
              />
              <h3 class="mt-5 mb-5 text-h5">{{ items.title }}</h3>
              <p>
                {{ items.content }}
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="service">
      <v-container class="">
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="service__heading text-center">
              <h2 class="mb-6 text-h4 white--text">Services</h2>
              <p class="mb-6 white--text text-h5 font-weight-light">
                We provide data products and services and this is how we
                work/our process:
              </p>
            </div>
          </v-col>
        </v-row>
        <v-row justify="center" align="center">
          <v-col
            v-for="item in servicesItems"
            :key="item.icon"
            cols="12"
            sm="6"
          >
            <div class="service__item text-center">
              <img class="service-thumb" :src="item.icon" :alt="item.title" />
              <h3 class="mb-6 text-h5">{{ item.title }}</h3>
              <p>
                {{ item.content }}
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="client section-space">
      <v-container class="">
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="client__heading section-heading text-center">
              <h2 class="mb-6 text-h4">Clients</h2>
            </div>
          </v-col>
        </v-row>
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="client__item text-center">
              <p class="text-h6 font-weight-light">
                Katshi Way Design Creative has launched in 2013 with several key
                clients in the mobile, marketing, financial services and gaming
                space. We believe in working with those who have a clear vision
                of what problems they want solved, an understanding of the
                quality required and a firm grasp on the business value that a
                solution will unlock.
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="contact section-space">
      <v-container class="">
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="contact__heading section-heading text-center">
              <h2 class="mb-8 text-h4">Ready to discuss your next project?</h2>
            </div>
            <div class="contact__item text-center">
              <v-btn
                to="/Contact"
                class="green white--text ma-2 mr-sm-8 pa-6"
                outlined
                rounded
                elevation="2"
                color="primary"
              >
                Request a Quote
              </v-btn>
              <v-btn
                to="/Contact"
                class="green--text ma-2 pa-6"
                outlined
                rounded
                elevation="2"
                color="primary"
              >
                Contact Us
              </v-btn>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  layout: 'MainPageLayout',

  data() {
    return {
      aboutItems: [
        {
          icon: require('@/assets/dev.png'),
          title: 'Development',
          content:
            'With the specs finalised, our development team begin iterating through the feature list, developing the software and conducting rigourous testing to ensure quality in-production.',
        },
        {
          icon: require('@/assets/spec.png'),
          title: 'Specification',
          content:
            'At Katshi Way Design Creative, it all begins with a specification. We prepare a functional and technical specification detailing the exact backlog of features required to complete delivery.',
        },
        {
          icon: require('@/assets/analysis.png'),
          title: 'Analysis & Operations',
          content:
            'Our Analysis and DevOps team monitors the development process throughout, and are able to provide documentation and analysis throughout the process, ensuring quality in-use.',
        },
      ],
      servicesItems: [
        {
          icon: require('@/assets/services-icon-systems-green.png'),
          title: 'Software Solutions',
          content: `Katshi Design offers bespoke software based on rigourous software quality models. Whether web, mobile or desktop, our software solutions are led by our belief in the power of data to both describe and demonstrate software in-use.`,
        },
        {
          icon: require('@/assets/services-icon-systems-green.png'),
          title: 'Systems Architecture',
          content: `Just as a building is defined first by its architect, and a suit by its tailor, a software system's entire presence and pattern is subject to the whim and wisdom of its architect. How can you ensure a quality software product? It all starts with the architecture.`,
        },
        {
          icon: require('@/assets/services-icon-tech-audit-green.png'),
          title: 'Technology Audit',
          content: `Are you concerned that the software and technology in your business is out of control? Have you lost faith and trust in those advising you on what to purchase and how to leverage your investments already made?`,
        },
        {
          icon: require('@/assets/services-icon-dev-review-green.png'),
          title: 'Developer Review',
          content:
            'Our Analysis and DevOps team monitors the development process throughout, and are able to provide documentation and analysis throughout the process, ensuring quality in-use.',
        },
      ],
    }
  },
}
</script>
<style lang="scss" scoped>
.hero {
  background-image: url('../assets/capetown.jpg');
  background-position: top center;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
  min-height: 31rem;
  position: relative;
  display: flex;
  align-items: center;
  color: #fff;
  padding: 100px 50px 50px;
  &__content {
    margin: auto;
  }
}

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
    h3 {
      color: #26b186;
      font-weight: 400;
    }
  }
}
.service {
  background: rgba(50, 50, 50, 0.7);
  padding: 100px 50px;
  &__item {
    background-color: #fff;
    border-radius: 5px;
    padding: 20px;
    transition: all 0.3s linear;
    position: relative;
    cursor: pointer;
    &:hover {
      box-shadow: 0 0 16px #3f4040;
    }
  }
  &-thumb {
    margin: 55px auto 40px;
  }
}

.section-space {
  padding: 100px 50px;
}

.client {
  background-image: url('../assets/global-back2a.jpg');
  background-position: top center;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
  min-height: 31rem;
  position: relative;
  display: flex;
  align-items: center;
  color: #fff;
}

.contact {
  background-color: #f7f7fd;
}
</style>
