<template>
  <v-app>
    <!-- <HeroComponent /> -->
    <PageLoader />

    <v-main>
      <!---------------------------------------------------- Navigation ------------------------------------------------------->
      <v-app-bar id="nav" app elevation="0">
        <v-img
          height="45"
          width="110"
          contain
          alt="Vbid Logo"
          tile="true"
          class="reponsive pt-1 pb-1"
          src="https://vbid.app/vbid_logo_black.webp"
        ></v-img>
        <v-tabs center-active centered active-class="active-tab" class="">
          <v-tab href="#blogs" class="hidden-xs-only">Blogs</v-tab>
          <v-tab href="#uudai" class="hidden-xs-only">Ưu Đãi</v-tab>
          <v-tab href="#vbid" class="hidden-xs-only">Về VBID</v-tab>
          <v-tab href="#chinhsach">Chính Sách</v-tab>
          <v-tab href="#trogiup">Trợ Giúp</v-tab>
        </v-tabs>

        <v-btn
          large
          elevation="1"
          background="rgba(255, 255, 255, 0.5)"
          class="black--text ml-3 px-5 hidden-xs-only"
          >Đăng nhập</v-btn
        >
        <v-btn
          large
          elevation="1"
          color="pink"
          class="white--text ml-3 px-5 hidden-xs-only"
          >Đăng kí
        </v-btn>
      </v-app-bar>

      <video id="inspire" src="../public/car.mp4" autoplay muted loop></video>

      <!----------------------------------------------------  ------------------------------------------------------->
      <section class="glass-bg">
        <v-row class="align-center px-10">
          <v-col cols="12" lg="6" class="pa-6 font-weight-bold py-16">
            <h2 class="display-3" data-aos="fade-up" data-aos-delay="400">
              Hợp tác với những người thuận lợi!
            </h2>

            <v-row class="pt-16">
              <v-subheader data-aos="fade-up" data-aos-delay="500"
                >VBID là nền tảng kết nối chủ xe và khách thuê một cách nhanh
                chóng với mức chiết khấu chỉ 5% cho mỗi giao dịch thành
                công..</v-subheader
              >
            </v-row>

            <br />
            <br />

            <v-btn
              large
              elevation="5"
              color="#32A071"
              class="white--text ml-10 px-5 py-5"
              >Trở thành đối tác VBID
            </v-btn>
          </v-col>
          <v-col lg="6" cols="12">
            <v-img
              data-aos="fade-left"
              data-aos-delay="500"
              class="pa-10"
              height="450"
              src="https://hopnhatgroup.com/public/cuploads/images/hop-tac.jpg"
            >
            </v-img>
          </v-col>
        </v-row>
      </section>

      <!---------------------------------------------------- ------------------------------------------------------->
      <section id="uudai" class="glass-bg">
        <v-row justify="center" class="align-center">
          <v-col sm="6" cols="12">
            <v-card
              data-aos="fade-right"
              data-aos-delay="600"
              class="text-center pa-6 rounded-lg"
              color="#e1e0e0c9"
              elevation="6"
            >
              <v-icon left size="20">mdi-account</v-icon>
              <v-card-subtitle class="green--text"
                >Người giới thiệu<br />
                Họ giao dịch, bạn kiếm được!
              </v-card-subtitle>

              <h4 class="display-0 font-weight-regular">
                Giới thiệu khách hàng với chúng tôi và nhận được khoản giảm giá
                trên số lượng họ giao dịch.
              </h4>

              <v-form>
                <ul style="list-style-type: none">
                  <li>
                    <p>
                      <v-icon>mdi-check</v-icon>FX Majors: Receive up to $35 per
                      million US$ traded
                    </p>
                  </li>
                  <li style="">
                    <p>
                      <v-icon>mdi-check</v-icon>FX Minors and Exotics: Receive
                      up to $45 per million US$ traded
                    </p>
                  </li>
                  <li style="">
                    <p>
                      <v-icon>mdi-check</v-icon>Customised rebate schemes
                      tailored just for you!
                    </p>
                  </li>
                </ul>
              </v-form>

              <v-btn
                large
                elevation="5"
                color="pink"
                class="white--text mt-10 px-10 py-5"
                >Trở thành người giới thiệu
              </v-btn>
            </v-card>
          </v-col>

          <v-col sm="6" cols="12">
            <v-card
              data-aos="fade-left"
              data-aos-delay="600"
              class="text-center pa-6 rounded-lg"
              color="#e1e0e0c9"
              elevation="6"
            >
              <v-icon left size="20">mdi-account</v-icon>
              <v-card-subtitle class="green--text"
                >Chi nhánh<br />
                Họ đăng ký, bạn kiếm được!!
              </v-card-subtitle>

              <h4 class="display-0 font-weight-regular">
                Được trả tiền cho mỗi khách hàng mở tài khoản với chúng tôi.
              </h4>

              <v-form>
                <ul style="list-style-type: none">
                  <li>
                    <p>
                      <v-icon>mdi-check</v-icon>Nhận tới $ 1,100 cho mỗi khách
                      hàng mà bạn giới thiệu cho VBID.
                    </p>
                  </li>
                  <li style="">
                    <p>
                      <v-icon>mdi-check</v-icon>Các chương trình hoa hồng phù
                      hợp với nhu cầu cá nhân.
                    </p>
                  </li>
                  <li style="">
                    <p>
                      <v-icon>mdi-check</v-icon>Tăng mạng lưới toàn cầu của bạn
                      với các tài liệu tiếp thị độc quyền.
                    </p>
                  </li>
                </ul>
              </v-form>

              <v-btn
                large
                elevation="5"
                color="pink"
                class="white--text mt-10 px-10 py-5"
                @click="check"
                >Trở thành cộng tác viên
              </v-btn>
            </v-card>
          </v-col>
        </v-row>
      </section>
      <!---------------------------------------------------- Navigation ------------------------------------------------------->
      <section class="glass-bg" id="vbid">
        <v-card
          class="text-center pa-6 rounded-lg"
          color="#e1e0e0c9"
          elevation="0"
        >
          <h6
            class="display-2 text-center"
            data-aos="fade-down"
            data-aos-delay="400"
          >
            Giới thiệu mạng lưới khách hàng của bạn với nhà môi giới số 1 thế
            giới.
          </h6>

          <v-card-subtitle
            class="green--text"
            data-aos="fade-down"
            data-aos-delay="500"
            >Điền thông tin chi tiết của bạn vào bên dưới và chúng tôi sẽ liên
            hệ với bạn.
          </v-card-subtitle>

          <v-row justify="center">
            <v-col cols="12" sm="10" md="8" lg="6">
              <v-card ref="form" data-aos="fade-down" data-aos-delay="600">
                <v-card-text>
                  <p style="text-align: left">Loại quan hệ đối tác của bạn</p>
                  <v-row>
                    <v-col cols="2">
                      <v-checkbox
                        label="IB"
                        value="IB"
                        id="IB"
                        ref="IB"
                      ></v-checkbox>
                    </v-col>
                    <v-col>
                      <v-checkbox label="Chi Nhánh" value="Chi nhánh">
                      </v-checkbox>
                    </v-col>
                  </v-row>
                  <v-text-field
                    ref="account"
                    v-model="account"
                    label="Số tài khoản(nếu có)"
                    placeholder=""
                  >
                  </v-text-field>
                  <p
                    style="
                      text-align: left;
                      color: #b68756;
                      text-transform: uppercase;
                    "
                  >
                    Thông tin liên lạc
                  </p>
                  <v-text-field
                    ref="name"
                    v-model="name"
                    :rules="[() => !!name || 'This field is mandatory']"
                    :error-messages="errorMessages"
                    label="Full Name"
                    placeholder="Diệu Mi"
                    required
                  ></v-text-field>

                  <v-text-field
                    ref="address"
                    v-model="address"
                    :rules="[
                      () => !!address || 'This field is mandatory.',
                      () =>
                        (!!address && address.length <= 25) ||
                        'Address must be less than 25 characters',
                      addressCheck,
                    ]"
                    label="Your contact number"
                    placeholder=""
                    counter="25"
                    required
                  ></v-text-field>

                  <v-text-field
                    ref="email"
                    v-model="email"
                    :rules="[
                      () => !!email || 'This field is mandatory.',
                      () =>
                        !!/.+@.+\..+/.test(email) ||
                        'Please enter a valid email address',
                    ]"
                    label="Enter your email"
                    placeholder="mitran.290901@gmail.com"
                    required
                  ></v-text-field>

                  <v-autocomplete
                    ref="country"
                    v-model="country"
                    :rules="[() => !!country || 'This field is mandatory.']"
                    :items="countries"
                    label="Country of residence"
                    placeholder="Select..."
                    required
                  ></v-autocomplete>

                  <v-text-field
                    ref="link"
                    v-model="link"
                    label="Website link (if available)"
                    required
                    placeholder=""
                  >
                  </v-text-field>
                  <v-textarea
                    name="note"
                    v-model="note"
                    :rules="[() => !!note || 'This field is mandatory.']"
                    label="Give further details about you activity:"
                    required
                  ></v-textarea>
                </v-card-text>

                <v-divider class="mt-12"></v-divider>

                <v-card-text>
                  Lưu ý: Xin lưu ý rằng nếu đơn đăng ký của bạn được thông qua,
                  bạn sẽ cần phải có một tài khoản được kích hoạt với VBID. Bạn
                  có thể mở một tài khoản từ <a href="#">đây</a>
                </v-card-text>

                <v-slide-x-reverse-transition>
                  <v-tooltip v-if="formHasErrors" left>
                    <template v-slot:activator="{ on, attrs }">
                      <v-btn
                        icon
                        class="my-0"
                        v-bind="attrs"
                        @click="resetForm"
                        v-on="on"
                      >
                        <v-icon>mdi-refresh</v-icon>
                      </v-btn>
                    </template>
                    <span>Refresh form</span>
                  </v-tooltip>
                </v-slide-x-reverse-transition>

                <v-btn
                  class="text-center px-6 rounded-lg"
                  large
                  elevation="5"
                  color="#B68756"
                  @click="submit"
                >
                  Submit
                </v-btn>

                <v-card-text>
                  Dữ liệu cá nhân của bạn sẽ được chúng tôi xử lý theo Chính
                  sách Bảo mật của chúng tôi có sẵn trên trang web của chúng
                  tôi.
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </v-card>
      </section>
      <!----------------------------------------------------  ------------------------------------------------------->
      <section class="glass-bg" id="chinhsach">
        <!-- <v-img
          class="pa-10"
          height="500"
          color="#e1e0e0c9"
          gradient="to bottom, rgb(200 200 180), rgb(227 227 227 / 55%)"
          src="https://designshack.net/wp-content/uploads/Home-office.jpg"
        > -->
        <div>
          <HeroComponent />
        </div>

        <v-row justify="center" class="align-center">
          <v-col sm="3" cols="12">
            <div class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
              <h3 class="black--text text-center display-0 font-weight-regular">
                Thanh Toán Trực Tuyến
              </h3>

              <v-card-subtitle class="text-center"
                >Chúng tôi làm việc với những chủ xe uy tín mang đến cho khách
                hàng nhiều lựa chọn khi thuê xe thông qua nền tảng VBID. Nhận
                báo giá thuê xe nhanh chóng, thanh toán trực tuyến an toàn.<br />
              </v-card-subtitle>
            </div>
          </v-col>

          <v-col sm="3" cols="12">
            <div class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
              <h3 class="black--text text-center display-0 font-weight-regular">
                Giá trị VBID đem lại.
              </h3>

              <v-card-subtitle class="text-center"
                >VBID cam kết mang đến những trải nghiệm tuyệt vời cho khách
                hàng bao gồm 4 giá trị nền tảng Value/Chất lượng -- Best
                price/Giá tốt nhất -- Integrity/Trung thực -- Delight/Vui vẻ.<br />
              </v-card-subtitle>
            </div>
          </v-col>

          <v-col sm="3" cols="12">
            <div class="pa-6 rounded-lg" color="#e1e0e0c9" elevation="6">
              <h3 class="black--text text-center display-0 font-weight-regular">
                An toàn cho mỗi chuyến đi.
              </h3>
              <v-card-subtitle class="text-center"
                >Với VBID người dùng thuê xe an toàn và tiết kiệm hơn. Mục tiêu
                mở rộng dịch vụ cho thuê xe tại 63 tỉnh thành, VBID hứa hẹn mang
                đến cho khách hàng những trải nghiệm tuyệt vời nhất.<br />
              </v-card-subtitle>
            </div>
          </v-col>
        </v-row>
        <!-- </v-img> -->
      </section>
    </v-main>
    <!----------------------------------------------------------------------------------------------------------->
    <section class="bg1">
      <!-- <v-img
        class=" pt-10"
        height="550"
        gradient="to bottom, rgb(166 199 156), rgb(227 227 227 / 40%)"
        src="https://img.freepik.com/free-photo/contact-us_36325-2135.jpg?size=626&ext=jpg"
      > -->
      <v-container>
        <v-divider />
        <br />
        <v-row>
          <v-col align="center" sm="3" md="2" cols="12">
            <v-img
              height="45"
              width="110"
              contain
              src="https://vbid.app/vbid_logo_black.webp"
              data-aos="fade-down"
              data-aos-delay="400"
            >
            </v-img>

            <a
              href="https://www.facebook.com/VBIDapp"
              target="_blank"
              class="
                v-btn v-btn--icon v-btn--round
                theme--light
                v-size--default
              "
              style="color: #ef7d58"
            >
              <span class="v-btn__content">
                <i
                  aria-hidden="true"
                  class="v-icon notranslate mdi mdi-facebook theme--light"
                >
                </i>
              </span>
            </a>

            <a
              href="https://www.instagram.com/vbid.app/"
              target="_blank"
              class="
                v-btn v-btn--icon v-btn--round
                theme--light
                v-size--default
              "
              style="color: #ef7d58"
              ><span class="v-btn__content"
                ><i
                  aria-hidden="true"
                  class="v-icon notranslate mdi mdi-instagram theme--light"
                >
                </i>
              </span>
            </a>

            <a
              href="https://www.linkedin.com/company/vbid-vietnam-jsc"
              target="_blank"
              class="
                v-btn v-btn--icon v-btn--round
                theme--light
                v-size--default
              "
              style="color: #ef7d58"
              ><span class="v-btn__content"
                ><i
                  aria-hidden="true"
                  class="v-icon notranslate mdi mdi-linkedin theme--light"
                ></i>
              </span>
            </a>
          </v-col>

          <v-col align="center" cols="6" sm="3">
            <div class="text-h5" style="cursor: pointer">Về VBID</div>
          </v-col>

          <v-col align="center" cols="6" lg="3">
            <div class="text-h5">Chính Sách</div>
            <div>
              Chính Sách Bảo mật thông tin<br />Giải quyết tranh chấp<br />Blogs
            </div>
          </v-col>
          <v-col align="center" cols="12" sm="3" md="4">
            <div class="text-h5">Liên Hệ</div>
            <div>
              0839991506<br />
              support@vbid.app<br />
              Trụ sở chính Tầng 14, Tòa Nhà HM Town 412 Nguyễn Thị Minh Khai
              Phường 05, Quận 03 Thành Phố Hồ Chí Minh
            </div>

            <v-card-actions> </v-card-actions>
          </v-col>
        </v-row>
      </v-container>

      <div class="">
        <v-col
          class="text-center"
          cols="12"
          style="background-color: #e1e0e0c9"
        >
          <strong
            >©{{ new Date().getFullYear() }} - Copyright VBID All rights
            reserved
          </strong>
        </v-col>
      </div>

      <!-- </v-img> -->
    </section>

    <v-bottom-navigation
      class="hidden-lg-only"
      style="position: fixed"
      v-model="value"
    >
      <v-btn value="home" style="color: #ef7d58">
        <span>Trang chủ</span>

        <v-icon>mdi-home</v-icon>
      </v-btn>

      <v-btn value="blogs">
        <span>Blogs</span>

        <v-icon>mdi-book-information-variant</v-icon>
      </v-btn>

      <v-btn value="account">
        <span>Tài Khoản</span>

        <v-icon>mdi-account</v-icon>
      </v-btn>
    </v-bottom-navigation>
  </v-app>
</template>

<script>
import HeroComponent from "./components/HeroComponent.vue";

import PageLoader from "./components/PageLoader.vue";
export default {
  name: "App",
  data: () => ({
    value: "home",
    isActive: false,
    countries: [
      "Afghanistan",
      "Albania",
      "Algeria",
      "Andorra",
      "Angola",
      "Anguilla",
      "Antigua &amp; Barbuda",
      "Argentina",
      "Armenia",
      "Aruba",
      "Australia",
      "Austria",
      "Azerbaijan",
      "Bahamas",
      "Bahrain",
      "Bangladesh",
      "Barbados",
      "Belarus",
      "Belgium",
      "Belize",
      "Benin",
      "Bermuda",
      "Bhutan",
      "Bolivia",
      "Bosnia &amp; Herzegovina",
      "Botswana",
      "Brazil",
      "British Virgin Islands",
      "Brunei",
      "Bulgaria",
      "Burkina Faso",
      "Burundi",
      "Cambodia",
      "Cameroon",
      "Cape Verde",
      "Cayman Islands",
      "Chad",
      "Chile",
      "China",
      "Colombia",
      "Congo",
      "Cook Islands",
      "Costa Rica",
      "Cote D Ivoire",
      "Croatia",
      "Cruise Ship",
      "Cuba",
      "Cyprus",
      "Czech Republic",
      "Denmark",
      "Djibouti",
      "Dominica",
      "Dominican Republic",
      "Ecuador",
      "Egypt",
      "El Salvador",
      "Equatorial Guinea",
      "Estonia",
      "Ethiopia",
      "Falkland Islands",
      "Faroe Islands",
      "Fiji",
      "Finland",
      "France",
      "French Polynesia",
      "French West Indies",
      "Gabon",
      "Gambia",
      "Georgia",
      "Germany",
      "Ghana",
      "Gibraltar",
      "Greece",
      "Greenland",
      "Grenada",
      "Guam",
      "Guatemala",
      "Guernsey",
      "Guinea",
      "Guinea Bissau",
      "Guyana",
      "Haiti",
      "Honduras",
      "Hong Kong",
      "Hungary",
      "Iceland",
      "India",
      "Indonesia",
      "Iran",
      "Iraq",
      "Ireland",
      "Isle of Man",
      "Israel",
      "Italy",
      "Jamaica",
      "Japan",
      "Jersey",
      "Jordan",
      "Kazakhstan",
      "Kenya",
      "Kuwait",
      "Kyrgyz Republic",
      "Laos",
      "Latvia",
      "Lebanon",
      "Lesotho",
      "Liberia",
      "Libya",
      "Liechtenstein",
      "Lithuania",
      "Luxembourg",
      "Macau",
      "Macedonia",
      "Madagascar",
      "Malawi",
      "Malaysia",
      "Maldives",
      "Mali",
      "Malta",
      "Mauritania",
      "Mauritius",
      "Mexico",
      "Moldova",
      "Monaco",
      "Mongolia",
      "Montenegro",
      "Montserrat",
      "Morocco",
      "Mozambique",
      "Namibia",
      "Nepal",
      "Netherlands",
      "Netherlands Antilles",
      "New Caledonia",
      "New Zealand",
      "Nicaragua",
      "Niger",
      "Nigeria",
      "Norway",
      "Oman",
      "Pakistan",
      "Palestine",
      "Panama",
      "Papua New Guinea",
      "Paraguay",
      "Peru",
      "Philippines",
      "Poland",
      "Portugal",
      "Puerto Rico",
      "Qatar",
      "Reunion",
      "Romania",
      "Russia",
      "Rwanda",
      "Saint Pierre &amp; Miquelon",
      "Samoa",
      "San Marino",
      "Satellite",
      "Saudi Arabia",
      "Senegal",
      "Serbia",
      "Seychelles",
      "Sierra Leone",
      "Singapore",
      "Slovakia",
      "Slovenia",
      "South Africa",
      "South Korea",
      "Spain",
      "Sri Lanka",
      "St Kitts &amp; Nevis",
      "St Lucia",
      "St Vincent",
      "St. Lucia",
      "Sudan",
      "Suriname",
      "Swaziland",
      "Sweden",
      "Switzerland",
      "Syria",
      "Taiwan",
      "Tajikistan",
      "Tanzania",
      "Thailand",
      `Timor L'Este`,
      "Togo",
      "Tonga",
      "Trinidad &amp; Tobago",
      "Tunisia",
      "Turkey",
      "Turkmenistan",
      "Turks &amp; Caicos",
      "Uganda",
      "Ukraine",
      "United Arab Emirates",
      "United Kingdom",
      "United States",
      "Uruguay",
      "Uzbekistan",
      "Venezuela",
      "VietNam",
      "Virgin Islands (US)",
      "Yemen",
      "Zambia",
      "Zimbabwe",
    ],

    errorMessages: "",
    account: null,
    name: null,
    address: null,
    email: null,
    country: null,
    link: null,
    note: null,
    formHasErrors: false,
  }),

  components: {
    HeroComponent,
    PageLoader,
  },

  computed: {
    form() {
      return {
        account: this.account,
        name: this.name,
        address: this.address,
        email: this.email,
        country: this.country,
        link: this.link,
        note: this.note,
      };
    },
  },

  watch: {
    name() {
      this.errorMessages = "";
    },
  },

  methods: {
    addressCheck() {
      this.errorMessages =
        this.address && !this.name ? `Hey! I'm required` : "";

      return true;
    },

    resetForm() {
      this.errorMessages = [];
      this.formHasErrors = false;

      Object.keys(this.form).forEach((f) => {
        this.$refs[f].reset();
      });
    },

    submit() {
      this.formHasErrors = false;

      Object.keys(this.form).forEach((f) => {
        if (!this.form[f]) this.formHasErrors = true;

        this.$refs[f].validate(true);
      });
    },

    //xử lý event
    check() {
      console.log(this.$refs.ib);
    },
  },

  // sliders: [
  //   "https://cdn.searchenginejournal.com/wp-content/uploads/2020/01/which-web-design-platform-is-right-for-you-5e4d59fb941b9-1520x800.png",
  //   "https://cdn.searchenginejournal.com/wp-content/uploads/2019/12/5-ways-seo-web-design-go-together-5e2945dd5df37.png",
  //   "https://data.whicdn.com/images/350420216/original.jpg?t=1605047796",
  //   "https://1zylgb20pxi7mw2sdr8i4a14-wpengine.netdna-ssl.com/wp-content/uploads/2020/01/projectleft.jpg",
  //   "https://cdn.dribbble.com/users/702789/screenshots/14012516/media/561a8b7e8cbe51c72c18f4ef0dc72676.png?compress=1&resize=400x300",
  //   "https://cdn.dribbble.com/users/2399102/screenshots/15522177/media/346d890482d929610d316938e7d48629.png?compress=1&resize=400x300",
  // ],
};
</script>






<style>
#inspire {
  position: fixed;
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
  object-position: center;
  z-index: -1;
  top: 0;
  left: 0;
}
.bg {
  width: 100%;
  height: 100%;
  display: block;
  background: rgba(255, 255, 255, 0.5);

  backdrop-filter: blur(5px);
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
  justify-content: center;

  align-items: center;
}
.bg1 {
  width: 100%;

  height: 100%;
  background: rgba(33, 170, 180, 0.634);
}
.glass-bg {
  width: 1000px;
  /* height: 600px; */
  max-width: 100%;
  display: block;
  margin: 80px 0px;
  margin-left: auto;
  margin-right: auto;

  background: rgba(255, 255, 255, 0.5);
  backdrop-filter: blur(2px);
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.4);
  /* display: flex; */
  justify-content: center;
  align-items: center;
}

.v-tab.active-tab {
  color: #e91e63;
}

.v-tab.active-tab::before {
  background-color: #4caf50;
}

@media screen and (max-width: 320px) {
}
</style>

