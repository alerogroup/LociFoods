<template>
  <v-footer dark color="#DBF3FA" class="mt-8" >
      <v-layout column mt-3>
        <v-row>
          <v-col>
            <v-row>
               <v-layout column ml-12>
                   <a href="#home" class="links_item_footer">Home</a>
                   <a href="#aboutus" class="links_item_footer">About us</a>
                   <a href="#ourproducts" class="links_item_footer">Our Products</a>
               </v-layout>
            </v-row>
          </v-col>
          <v-col>
            <v-row>
               <v-layout column ml-3>
                  <a href="#contactus" class="links_item_footer">Contact us</a>
                  <router-link to="/policy" class=" links_item_footer">Privacy Policy</router-link>
               </v-layout>
            </v-row>
          </v-col>
           </v-row>
        <v-layout>
        <p class="copyright links_item_footer">Copyright &copy; Loci Foods
        </p>
        <v-spacer />
        <v-layout justify-end class="ml-7">
            <div class="ig">
              <a href="https://instagram.com/loci_foods?igshid=1feazc81jqwtr"><img class="ml-4" :src="instagram" alt="instagram"></a>
            </div>
            <div class="linkedin">
                <a href="https://ke.linkedin.com/in/loci-foods-067062193"><img class="ml-4" :src="linkedIn" alt="linkedIn"></a>
            </div>
            <div class="linkedin">
                <a href="mailto:locifoods@gmail.com"><img class="ml-4" :src="mail" alt="email"></a>
            </div>
        </v-layout>
        </v-layout>
      </v-layout>
  </v-footer>
</template>

<script>
const IMAGEKIT_BASE_URL = 'https://ik.imagekit.io/qpt2onjfe/'

export default {
  data: () => ({
    instagram: IMAGEKIT_BASE_URL + 'images/instagram_u1C6-uS8w.svg',
    linkedIn: IMAGEKIT_BASE_URL + '/loci/images/linkedin_-SuwW-mt7.svg',
    mail: IMAGEKIT_BASE_URL + '/loci/images/icons/email_aWqtcW4Rtg.svg',
    w: '70'
  })
}
</script>
