<template>
  <div>
    <Banner :title="banner.title" :description="banner.description" />
    <div class="section-space">
      <v-container>
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="about__heading">
              <h2 class="d-flex justify-center align-center mb-8 text-h4">
                <img
                  :src="require('~/assets/services-icon-software.png')"
                  alt="Software Solutions"
                /><span>Software Solutions</span>
              </h2>
              <p>
                If you've commissioned a software solution in the past, your
                experience is most likely a combination of frustration at a
                flawed product, along with a degree of satisfaction that a
                problem has been solved in a way that no off the shelf product
                could achieve.
              </p>
              <p>
                How can businesses gain a competitive advantage through their
                own software without unreasonable risk? The answer lies in a
                software of measurable quality.
              </p>
              <p>
                Full Stack offers bespoke software based on rigourous software
                quality models. Whether web, mobile or desktop, our software
                solutions are led by our belief in the power of data to both
                describe and demonstrate software in-use. The software solutions
                team measure and deliver on:
              </p>
              <ul>
                <li>The quality of software in-design [Planning]</li>
                <li>The quality of software in-production [Build]</li>
                <li>The quality of software in-use [Live Use]</li>
              </ul>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="client section-space">
      <v-container>
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="about__heading white--text">
              <h2 class="d-flex justify-center align-center mb-8 text-h4">
                <img
                  :src="require('~/assets/services-icon-systems-orange.png')"
                  alt="Systems Architecture"
                /><span class="white--text">Systems Architecture</span>
              </h2>
              <p>
                Just as a building is defined first by its architect, and a suit
                by its tailor, a software system's entire presence and pattern
                is subject to the whim and wisdom of its architect. How can you
                ensure a quality software product? It all starts with the
                architecture.
              </p>
              <p>
                How can you ensure that your system's architecture is of a high
                quality? Let Full Stack provide our detailed levels of technical
                and functional specification that we perform prior to the
                commencement of our own projects with your problem set.
              </p>
              <p>
                Whether an existing piece of software, or a new build, let Full
                Stack provide you with insights into your problem set, along
                with proposed solutions to ensure that your investment in
                software has a high return.
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="section-space">
      <v-container>
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="about__heading">
              <h2 class="d-flex justify-center align-center mb-8 text-h4">
                <img
                  :src="require('~/assets/services-icon-tech-audit.png')"
                  alt="Technology Audit"
                /><span>Technology Audit</span>
              </h2>
              <p>
                Are you concerned that the software and technology in your
                business is out of control? Have you lost faith and trust in
                those advising you on what to purchase and how to leverage your
                investments already made?
              </p>
              <p>
                As our core belief is in the power of software to enable
                competitive advantage, we aid organisations to leverage
                technology. Often we do this via the provision of an independent
                assessment of the technology in-use or planned within an
                organisation.
              </p>
              <p>
                This can be an important tool to make the right investments.
                With over three decade sof executive experience in technology,
                we can help provide an independent view on the systems and
                services powering your business, either prior to new investments
                or to assess ROI on past investments.
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <div class="contact section-space">
      <v-container>
        <v-row justify="center" align="center">
          <v-col cols="12">
            <div class="about__heading">
              <h2 class="d-flex justify-center align-center mb-8 text-h4">
                <img
                  :src="require('~/assets/services-icon-dev-review-orange.png')"
                  alt="Developer Sessions"
                /><span>Developer Sessions</span>
              </h2>
              <p>
                Does your development team need a refresh? Are your in-house
                resources feeling downtrodden or have lost motivation? Do they
                need to be inspired and receive a booster-shot of industry
                leading practices to improve their output?
              </p>
              <p>
                We want businesses to feel the power of software to unlock value
                through high quality software. We work hard every day to do that
                for our clients and ourselves.
              </p>
              <p>
                To do that, we are more than happy to work with in-house
                development teams to diagnose problems and encourage uptake of
                best practices in terms of methodology, technology stack and
                work behaviour. We don't have all the answers - however, as a
                passionate developer-led company we might have just the right
                patterns, play and practices to extract greater productivity and
                passion from your development team.
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
  name: 'IndexPage',
  components: { Banner },
  layout: 'MainPageLayout',
  data() {
    return {
      banner: {
        title: 'Services',
        description: `We love to serve our clients. These are the services we happily
                provide.`,
      },
    }
  },
}
</script>
<style lang="scss" scoped>
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
