<script lang="ts" setup>
import ChipToggle from './components/ChipToggle.vue';
import NavBar from './components/NavBar.vue';
import { Icon } from '@iconify/vue';

</script>

<template>
  <div>
    <div class="body-wrapper">
      <NavBar />
      <div class="header-description">
        <div class="main-header-wrapper">
          <p class="description-tags main-header"> An AI that can predict<br> diseases of your patients</p>

          <p class="description-tags sub-header"> and help cure them InTime </p>
        </div>
        <a href="#bookdemo"> <button class="description-tags btn" onclick="#solutions">Book A Demo</button></a>
        <p class="description-tags sub-text">Discover Our Solutions For<br> Business And Doctors</p>
        <div style="padding-bottom: 2rem;">
          <Icon icon='fa6-solid:angle-down' width="25" opacity="0.8" />
          <br>
          <Icon icon='fa6-solid:angle-down' width="15" opacity="0.6" />
        </div>
      </div>

    </div>
    <div class="section-headers">
      <div class="use-cases-wrapper">
        <h1>Use Cases</h1>
        <div class="use-cases-inner-wrapper">
          <div class="use-cases-left">
            <div class="use-cases-tl">
              <p>Use our app to get insights and track your health in the palm of your hand, or tough your browser</p>
              <div class="use-cases-icons-wrapper">
                <h1 class="big-section">For People</h1>
                <Icon class="use-cases-icons" icon="material-symbols:arrow-outward-rounded" width="30" />
              </div>
            </div>
            <div class="use-cases-bl">
              <p>Boost your doctor needs and quickly get biomarkers to run diagnosis</p>
              <div class="use-cases-icons-wrapper">
                <h1 class="small-section"> For Clinics And<br> Doctors</h1>
                <Icon class="use-cases-icons" icon="material-symbols:arrow-outward-rounded" width="30" />
              </div>
            </div>
          </div>
          <div class="use-cases-right">
            <div class="use-cases-tr">
              <p>Create and use custom AI models to diagnose your patients using our platform</p>
              <div class="use-cases-icons-wrapper">
                <h1 class="small-section"> For Hospitals</h1>
                <Icon class="use-cases-icons" icon="material-symbols:arrow-outward-rounded" width="30" />
              </div>
            </div>
            <div class="use-cases-br">
              <p>Manage multiple orgnizations in our panel with unlimited custom models and doctors {more text to be
                added}</p>
              <div class="use-cases-icons-wrapper">
                <h1 class="big-section"><br>For Organizations</h1>
                <Icon class="use-cases-icons" icon="material-symbols:arrow-outward-rounded" width="30" />
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="use-cases-wrapper">
        <h1 id="solutions">Solutions</h1>
        <div>
          <h2 class="solutions-headers">Solutions / <span style="color: #3683FC;"> APIs </span></h2>
        </div>
        <ChipToggle />
        <div>
          <h2 class="solutions-headers"> Solutions / <span style="color: #3683FC;"> App </span></h2>
        </div>
        <div class="solution-sections-wrappers">
          <div>
            <img src="../src/assets/Phone.png" class="solution-img">
          </div>
          <div>
            <h2>Patient connector</h2>
            <p class="solution-section-info">Connect to your patients trough our app to request data, chat and keep them
              informed since first visit</p>
            <a class="solutions-learn-more">Learn More
              <Icon class="small-icon-learn-more" icon="material-symbols:arrow-outward-rounded" width="20" />
            </a>
          </div>
        </div>
        <div>
          <h2 class="solutions-headers">Solutions / <span style="color: #3683FC;"> Simulation</span></h2>
        </div>
        <div class="solution-sections-wrappers">
          <div>
            <img src="../src/assets/Vector.png" class="solution-img">
          </div>
          <div>
            <h2>Simulation of Clinical trials with AI</h2>
            <p class="solution-section-info">Using AI algorithms we simulate effects of drugs and chnage of habits to
              give personalized results for patient biomarkers</p>
            <a class="solutions-learn-more">Learn More
              <Icon class="small-icon-learn-more" icon="material-symbols:arrow-outward-rounded" width="20" />
            </a>
          </div>
        </div>
      </div>

      <div class="use-cases-wrapper">
        <h1 id="pricing">Pricing</h1>
        <div class="pricing-section">
          <div class="pricecard-outer-wrapper">
            <div class="pricecard-wrapper">
              <div>
                <h2>Starter</h2>
                <p>Boost your clinic exams with fast diagnosis with help of AI</p>
              </div>
              <div class="pricing-list-wrapper">
                <ul class="pricing-list">
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png"> Predictions
                  </li>
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png">
                    Depersonalization</li>
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png"> Data
                    Structuring</li>
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png"> up to 5
                    doctors</li>
                </ul>
              </div>
              <div class="pricing-price">
                <p class="pricing-price-country">USD</p>
                <p class="pricing-price-amount">$39</p>
                <p class="pricing-price-time">/mo</p>
              </div>
            </div>
          </div>

          <div class="pricecard-outer-wrapper">
            <div class="pricecard-wrapper">
              <div>
                <h2>Professional</h2>
                <p>For Clinics and hospitals that want to giver personalized experience</p>
              </div>
              <div class="pricing-list-wrapper">
                <ul class="pricing-list">
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png"> All in
                    starter
                  </li>
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png">
                    10 Custom models</li>
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png"> Data
                    100 doctors</li>

                </ul>
              </div>
              <div class="pricing-price-2">
                <p class="pricing-price-country">USD</p>
                <p class="pricing-price-amount">$99</p>
                <p class="pricing-price-time">/mo</p>
              </div>
            </div>
          </div>

          <div class="pricecard-outer-wrapper">
            <div class="pricecard-wrapper">
              <div>
                <h2>Enterprise</h2>
                <p>For organizations that need powerful tools and custom services</p>
              </div>
              <div class="pricing-list-wrapper">
                <ul class="pricing-list">
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png"> All in
                    professional
                  </li>
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png">
                    Unlimited models and doctors</li>
                  <li class="pricing-list"> <img class="pricing-img-list" src="../src/assets/checkmark.png">
                    Multiple organizations panel</li>

                </ul>
              </div>
              <div class="pricing-price">
                <button class="pricing-btn">Contact Sales</button>
              </div>
            </div>
          </div>
        </div>
        <a class="pricing-navlink" href="">Full Pricing Table
          <Icon class="small-icon-arrows" icon="material-symbols:arrow-outward-rounded" width="20" />
        </a>
      </div>
    </div>

    <div class="body-wrapper">
      <div class="book-demo-header">
        <h1 id="bookdemo">Book A Demo</h1>
        <div class="book-message-container">
          <div>
            <textarea rows="12" class="book-message-field" type="text" placeholder="Message"></textarea>
          </div>
          <div class="book-demo-input-wrapper">
            <form class="book-demo-form">
              <div class="book-demo-input-inner-wrapper">
                <input type="text" required class="book-demo-input" placeholder="Name" id="name" name="name"
                  tabindex="1">
                <label class="book-demo-label" for="name">Name</label>
              </div>
              <div class="book-demo-input-inner-wrapper">
                <input type="email" required class="book-demo-input" placeholder="Email" id="email" name="email"
                  tabindex="2">
                <label class="book-demo-label" for="email">Email</label>
              </div>
              <div class="book-demo-input-inner-wrapper">
                <div class="book-demo-phone-wrapper">
                  <div>
                    <input type="text" required class="book-demo-input-cc" placeholder="+1" id="cc" name="cc"
                      tabindex="2">
                    <label class="book-demo-label-cc" for="cc"><img style="position: absolute;"
                        src="../src/assets/usflag.png" alt=""> <img src="../src/assets/usflag2.png" alt="" />
                    </label>
                  </div>
                  <div class="">
                    <input type="tel" required class="book-demo-input-phone" placeholder="Phone" id="Phone" name="phone"
                      tabindex="2">
                    <label class="book-demo-label" for="Phone">Phone</label>
                  </div>
                </div>
              </div>
            </form>
            <div class="book-demo-btn-wrapper">
              <button class="book-demo-btn">Send</button>
            </div>
          </div>
        </div>
        <div class="book-demo-contacts-wrapper">
          <div class="book-demo-email">
            <Icon icon="fa6-regular:envelope" width="30" color="#3683fc" />
            <p> business@longevityintime.org </p>
          </div>
          <div class="contacts-icon-links">
            <Icon class="contact-icons" icon="fa6-brands:twitter" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:facebook" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:linkedin" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:instagram" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:telegram" width="30" color="#3683fc" />
          </div>
        </div>
      </div>
    </div>

    <div id="footer" class="longevity-footer-wrapper">
      <img class="logo" src="./assets/Logo144.png">
      <div class="footer-content-wrapper">
        <div>
          <h2 class="footer-headers">InTime BioTech LLC.</h2>
          <p class="footer-contact-address">Dba. Longevity InTime <br> 300 Delaware Avenue, Suite 210-A, <br>
            Wilmington, Delaware, 19801, USA
          </p>
          <h2>Contact us</h2>
          <a style="text-decoration: none;" href="mailto:contact@intime.digital">
          <button class="footer-btn">Send A Message
            <Icon icon="material-symbols:arrow-outward-rounded" width="30" />
          </button>
        </a>
          <div class="book-demo-email">
            <Icon icon="fa6-regular:envelope" width="30" color="#3683fc" />
            <p class="footer-contact-email"> contact@intime.digital </p>
          </div>
          <div class="contacts-icon-links">
            <Icon class="contact-icons" icon="fa6-brands:twitter" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:facebook" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:linkedin" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:instagram" width="30" color="#3683fc" />
            <Icon class="contact-icons" icon="fa6-brands:telegram" width="30" color="#3683fc" />
          </div>
        </div>
        <div>
          <h2>Navigation</h2>
          <ul class="footer-list">
            <li>Home</li>
            <li>Reviews</li>
            <li>Who we are</li>
            <li>App</li>
            <li>Mission</li>
            <li>Partners</li>
            <li>Petition</li>
            <li>Books</li>
            <li>Carrers</li>
          </ul>
        </div>
        <div class="">
          <h2>Products & Services</h2>
          <ul class="footer-list">
            <li class="footer-list">Disease Tracker</li>
            <li>AntiCoronaVirus</li>
            <li>Longevity Petition</li>
            <li>Longevity Scientific Resort</li>
            <li>LongevityCoin ($LONG)</li>
            <li>Marketplace & NFTs</li>
            <li>Portable BioContainer</li>
            <li>Telemedicine</li>
            <li>Terms of Use</li>
            <li>Privacy Policy</li>
          </ul>
        </div>
      </div>
      <div class="bottom-footer-wrapper">
        <div class="play-store">
          <div class="play-store-wrapper">
            <img src="../src/assets/blackback.png" alt="">
            <img class="play-store-image" src="../src/assets/googlegroup.png" alt="">
          </div>
          <div class="play-store-wrapper">
            <img src="../src/assets/blackback.png" alt="">
            <img class="play-store-image" src="../src/assets/applegroup.png" alt="">
          </div>
        </div>
        <p>Powered by artificial intelligence, verified by scientists, generated by Big Data obtained from evidence
          based only clinical trials.</p>
      </div>
    </div>
    <div class="footer-waves">
      <img src="../src/assets/waves.png" alt="">
      <p class="footer-copyright">Copyright © 2018-2022, InTime BioTech LLC.</p>
    </div>
  </div>
</template>

<style scoped>

</style>
