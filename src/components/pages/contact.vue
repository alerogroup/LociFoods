<template>
<v-content>
     <v-layout column mt-8 class="hidden-sm-and-down">
        <v-flex xs12 md4>
        <v-layout column justify-center align-center>
            <div class="display-2 font-weight-light"> Contact Us</div>
            <v-row>
            <v-layout column justify-start>
                <v-flex xs12>
                  <a href="https://instagram.com/loci_foods?igshid=1feazc81jqwtr">
                  <v-row class="mt-6">
                    <img :src="icon_1" style="width:50px!important; height:50px!important">
                    <span class="mt-3 ml-4 links--text">loci_foods</span>
                  </v-row>
                  </a>
                </v-flex>
                <v-flex xs12>
                  <a href="https://ke.linkedin.com/in/loci-foods-067062193">
                    <v-row class="mt-6" >
                      <img :src="icon_2" style="width:50px!important; height:50px!important">
                      <span class="mt-3 ml-4 links--text">locifoods</span>
                    </v-row>
                  </a>
                </v-flex>
                <v-flex xs12>
                  <a href="mailto:locifoods@gmail.com" class="links--text">
                  <v-row class="mt-6">
                    <img :src="icon_3" style="width:50px!important; height:50px!important">
                    <span class="mt-3 ml-4">locifoods@gmail.com</span>
                  </v-row>
                  </a>
                </v-flex>
            </v-layout>
            <v-layout column ml-10 mt-8>
              <v-card flat width="400" class="ml-9" color="transparent">
                <p class="title font-weight-regular">Join our newsletter to get <br/> update & new release of <br /> the product</p>
                  <v-dialog v-model="dialog" width="500">
                    <template v-slot:activator="{ on }">
                        <v-btn color="secondary" dark v-on="on" width="200">
                          Get Started Here
                        </v-btn>
                    </template>
                    <v-card height="500">
                      <v-layout column justify-center align-center>
                        <v-card-title
                          class="display-1 font-weight-thin"
                          primary-title>
                             Stay informed
                        </v-card-title>
                        <p class="text-center">
                            We will keep you informed on news, <br> features of the app and more ...
                        </p>
                    <v-divider></v-divider>
                     <v-form
                        ref="form"
                        v-model="valid"
                        lazy-validation
                      >
                        <v-text-field
                           v-model="name"
                           :rules="nameRules"
                           label="Fullname"
                           filled
                           style="width:270px;"
                           color='secondary'
                           required>
                        </v-text-field>
                         <v-text-field
                           v-model="email"
                           :rules="nameRules"
                           label="Email"
                           filled
                           color='secondary'
                           required>
                        </v-text-field>
                    </v-form>
                      <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn large width="270" block color="secondary" @click="dialog = false" >
                        Next
                      </v-btn>
                  </v-card-actions>
                </v-layout>
              </v-card>
             </v-dialog>
           </v-card>
         </v-layout>
       </v-row>
     </v-layout>
   </v-flex>
 </v-layout>
  <!-- mobile phones -->
     <v-layout column mt-8 class="hidden-md-and-up">
        <v-flex xs12 md4>
        <v-layout column justify-center align-center>
            <div class="display-2 font-weight-light"> Contact Us</div>
            <v-row>
            <v-layout column justify-center ml-12>
                <v-flex xs12>
                  <a href="https://www.instagram.com/loci_foods/?igshid=1feazc81jqwtr">
                  <v-row class="mt-6 ml-12">
                    <img :src="icon_1" style="width:50px!important; height:50px!important">
                    <span class="mt-3 ml-4 links--text">loci_foods</span>
                  </v-row>
                  </a>
                </v-flex>
                <v-flex xs12>
                  <a href="https://ke.linkedin.com/in/loci-foods-067062193">
                    <v-row class="mt-6 ml-12" >
                      <img :src="icon_2" style="width:50px!important; height:50px!important">
                      <span class="mt-3 ml-4 links--text">locifoods</span>
                    </v-row>
                  </a>
                </v-flex>
                <v-flex xs12>
                  <a href="mailto:locifoods@gmail.com" class="links--text">
                  <v-row class="mt-6 ml-12">
                    <img :src="icon_3" style="width:50px!important; height:50px!important">
                    <span class="mt-3 ml-4">locifoods@gmail.com</span>
                  </v-row>
                  </a>
                </v-flex>
            </v-layout>
            <v-layout column ml-10 mt-8>
              <v-card flat width="400" class="ml-9" color="transparent">
                <p class="title font-weight-regular">Join our newsletter to get <br/> update & new release of <br /> the product</p>
                  <v-dialog v-model="dialog" width="500">
                    <template v-slot:activator="{ on }">
                        <v-btn color="secondary" dark v-on="on" width="200">
                          Get Started Here
                        </v-btn>
                    </template>
                    <v-card height="500">
                      <v-layout column justify-center align-center>
                        <v-card-title
                          class="display-1 font-weight-thin"
                          primary-title>
                             Stay informed
                        </v-card-title>
                        <p class="text-center">
                            We will keep you informed on news, <br> features of the app and more ...
                        </p>
                    <v-divider></v-divider>
                     <v-form
                        ref="form"
                        v-model="valid"
                        lazy-validation
                      >
                     <v-text-field
                           v-model="name"
                           :rules="nameRules"
                           label="Fullname"
                           filled
                           style="width:270px;"
                           color='secondary'
                           required>
                        </v-text-field>
                         <v-text-field
                           v-model="email"
                           :rules="nameRules"
                           label="Email"
                           filled
                           color='secondary'
                           required>
                        </v-text-field>
                    </v-form>
                      <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn large width="270" block color="secondary"  v-on:click="submit" type="submit">
                        Next
                      </v-btn>
                  </v-card-actions>
                </v-layout>
              </v-card>
             </v-dialog>
           </v-card>
         </v-layout>
       </v-row>
     </v-layout>
   </v-flex>
 </v-layout>

  <v-dialog
        v-model="dialogformSubmitted"
        width="400"
        v-if="formSubmitted"
      >
        <v-card width="auto" height="auto">
        <v-layout justify-center align-center>
           <v-card-text class="title font-weight-medium text-center pa-4">Thank you, <span class="name font-weight-medium">{{name}}</span> We have received your message and will get back to you</v-card-text>
        </v-layout>
      </v-card>
      </v-dialog>
</v-content>
</template>

<script>
const IMAGEKIT_BASE_URL = 'https://ik.imagekit.io/qpt2onjfe/'

export default {
  data: () => ({
    dialog: false,
    icon_1: IMAGEKIT_BASE_URL + '/images/mdi_insagram_GGDk8pV3i.png',
    icon_2: IMAGEKIT_BASE_URL + '/images/mdi_linkedin__U6Ub2uu8x.png',
    icon_3: IMAGEKIT_BASE_URL + '/images/mdi_email_BM05h89-xy.svg',
    name: '',
    email: '',
    dialogformSubmitted: false,
    formSubmitted: false,
    overlay: true
  }),
  watch: {
    overlay (val) {
      val && setTimeout(() => {
        this.overlay = false
      }, 3000)
    }
  },
  mounted () {
    this.$nextTick(function () {
      const emailJSscript = document.createElement('script')
      emailJSscript.setAttribute('src', 'https://cdn.emailjs.com/sdk/2.2.4/email.min.js')
      document.head.appendChild(emailJSscript)
    })
  },

  methods: {
    submit () {
      /* eslint-disable */
      const template_params = {
        'email': this.email,
        'name': this.name
      }
/* eslint-disable */
const service_id = "mailgun";
const template_id = "loci_foods";
      event.preventDefault()
      if (this.email !== null && this.name !== null) {
        this.formSubmitted = false
        this.dialogformSubmitted = false
        emailjs.init('user_c0Q2llk67OnYN7obTBRkR')
        this.contact_number = Math.random() * 100000 | 0
        emailjs.send(
          service_id, 
          template_id,
          template_params
        ).then((response) => {
          this.dialogformSubmitted = true
        
          console.log('SUCCESS You just sent an email...', response)
        }, (error) => {
          console.log('FAILED Throw an error to user...', error)
          this.isLoading = false
        })
      } else {
        //
      }
      this.$refs.form.reset(),
      this.dialog= false
    }
}
}

</script>
