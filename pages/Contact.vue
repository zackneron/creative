<template>
  <div>
    <Banner :title="banner.title" :description="banner.description" />
    <div class="contact section-space py-0">
      <v-container>
        <v-row justify="start" align="center">
          <v-col cols="12" sm="6" class="bg--lighten-blue">
            <div class="pt-16 px-10 pb-120">
              <span class="text-h5">Contact details</span>
              <v-card elevation="0" color="transparent">
                <v-list color="transparent">
                  <v-list-group value="collapse">
                    <template #activator>
                      <v-list-item-content>
                        <v-list-item-title class="text-h6 font-weight-light"
                          >Client Contact Centre</v-list-item-title
                        >
                      </v-list-item-content>
                    </template>

                    <v-list-item class="list-bg">
                      <v-list-item-icon>
                        <v-icon> mdi-phone </v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title>086 000 1111</v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>

                    <v-list-item class="list-bg">
                      <v-list-item-icon>
                        <v-icon> mdi-at </v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title
                          >support@katshiwaydesigncreative.co.za</v-list-item-title
                        >
                      </v-list-item-content>
                    </v-list-item>

                    <v-list-item class="mb-4">
                      <v-list-item-content>
                        <v-list-item-title class="text-caption"
                          >Monday - Friday 08:00 - 17:00</v-list-item-title
                        >
                        <v-list-item-subtitle class="text-caption"
                          >Closed on Saturday, Sunday and public
                          holidays</v-list-item-subtitle
                        >
                      </v-list-item-content>
                    </v-list-item>
                  </v-list-group>

                  <v-list-group>
                    <template #activator>
                      <v-list-item-content>
                        <v-list-item-title class="text-h6 font-weight-light"
                          >Head Office</v-list-item-title
                        >
                      </v-list-item-content>
                    </template>

                    <v-list-item class="list-bg">
                      <v-list-item-icon class="mr-4">
                        <v-icon> mdi-map-marker </v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title>2 StreetName Road</v-list-item-title>
                        <v-list-item-title>Location, Country</v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>

                    <v-list-item class="list-bg">
                      <v-list-item-icon class="mr-4">
                        <v-icon> mdi-email </v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title>PO Box 1</v-list-item-title>
                        <v-list-item-title
                          >PostslzCode, 7532
                        </v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>
                  </v-list-group>

                  <v-list-group>
                    <template #activator>
                      <v-list-item-content>
                        <v-list-item-title class="text-h6 font-weight-light"
                          >Other Office</v-list-item-title
                        >
                      </v-list-item-content>
                    </template>

                    <v-list-item class="list-bg">
                      <v-list-item-icon class="mr-4">
                        <v-icon> mdi-map-marker </v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title
                          >Name Office Park, Block D,
                        </v-list-item-title>
                        <v-list-item-title
                          >254 StreetName, City,</v-list-item-title
                        >
                        <v-list-item-title>Location, 0045</v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>

                    <v-list-item class="list-bg">
                      <v-list-item-icon class="mr-4">
                        <v-icon> mdi-email </v-icon>
                      </v-list-item-icon>
                      <v-list-item-content>
                        <v-list-item-title
                          >Private Bag X14, Postal,
                        </v-list-item-title>
                        <v-list-item-title>0000, Country</v-list-item-title>
                      </v-list-item-content>
                    </v-list-item>
                  </v-list-group>
                </v-list>
              </v-card>
            </div>
          </v-col>
          <v-col cols="12" sm="6">
            <div class="pt-16 px-10 pb-120">
              <v-card elevation="0">
                <span class="mb-2 d-block font-weight-bold black--text">
                  Full name
                </span>
                <v-card-text class="pa-0">
                  <v-text-field
                    v-model="fullName"
                    outlined
                    label="Full name"
                  ></v-text-field>
                </v-card-text>
              </v-card>

              <v-card elevation="0">
                <span class="mb-2 d-block font-weight-bold black--text">
                  Email
                </span>
                <v-card-text class="pa-0">
                  <v-text-field
                    v-model="email"
                    outlined
                    label="Email"
                  ></v-text-field>
                </v-card-text>
              </v-card>

              <v-card elevation="0">
                <span class="mb-2 d-block font-weight-bold black--text">
                  Contact number
                </span>
                <v-card-text class="pa-0">
                  <v-text-field
                    v-model="contactNumber"
                    outlined
                    label="Contact number"
                  ></v-text-field>
                </v-card-text>
              </v-card>

              <v-card elevation="0">
                <span class="mb-2 d-block font-weight-bold black--text">
                  Message
                </span>
                <v-card-text class="pa-0">
                  <v-textarea
                    v-model="messageBox"
                    auto-grow
                    outlined
                    label="Message"
                    value=""
                  >
                  </v-textarea>
                </v-card-text>
              </v-card>

              <v-card
                elevation="0"
                class="d-flex flex-column flex-md-row align-md-center"
              >
                <v-btn
                  to="/Contact"
                  class="green white--text ma-2 mr-sm-8 pa-6"
                  outlined
                  rounded
                  elevation="2"
                  color="primary"
                >
                  Submit
                </v-btn>
              </v-card>
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
        title: 'We are here to help',
        description: `Please fill out your details below so we can assist you with your general concerns.`,
      },
      fullName: '',
      email: '',
      contactNumber: '',
      messageBox: '',
    }
  },
}
</script>

<style lang="scss" scoped>
.contact {
  &-thumb {
    max-width: 77px;
    opacity: 0.5;
  }
  &__item {
    padding: 20px;
    &:hover {
      cursor: pointer;
      transition: all 0.5s ease-in;
      .contact-thumb {
        transform: scale(1.2);
        transition: all 0.3s ease-in;
      }
    }
  }
}

.section-space {
  padding: 100px 50px;
}

.v-application .v-list-group--active.primary--text {
  color: #4caf50 !important;
  caret-color: #4caf50 !important;
}
</style>
