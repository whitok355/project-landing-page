<template>
  <div class="b-wrapper">
    <div class="b-container b-relative b-padding">
      <div class="b-header">
        <logo></logo>
        <navigation></navigation>
        <us></us>
        <div class="b-img"></div>
      </div>
      <div class="b-helping">
        <div class="b-helping__content">
          <logo></logo>
          <div class="b-helping__title">HELPING YOU THRIVE IN ALL AREAS OF LIFE</div>
          <div
            class="b-helping__text"
          >Our highly talented therapists can help you with a range of issues including relationships, sex, PTSD, depression, social anxiety, or even just caring for yourself more.</div>
        </div>
        <div class="b-helping__boxBtn">
          <div class="b-helping__who" @mouseover="changeClass('who', 'what')">WHO AM I</div>
          <div class="b-helping__what" @mouseover="changeClass('what', 'who')">WHAT DO I DO</div>
        </div>
      </div>
    </div>
    <div class="b-container-why">
      <div class="b-container b-relative b-padding">
        <div class="b-why">
          <div class="b-why__title">Why Thrive?</div>
          <div
            class="b-why__text"
          >Want to improve your well-being from the comfort of your own couch? Are you having trouble finding the right therapist? Here at ThriveTalk, our licensed therapists provide the same quality care you would get in office from anywhere you can access your laptop or mobile phone. Become your best self with ThriveTalk. Start therapy now with a licensed therapist!</div>
          <div class="b-why__img"></div>
        </div>
      </div>
    </div>
    <div class="b-container b-padding">
      <div class="b-about">
        <div class="b-about__title">ABOUT US</div>
        <div
          class="b-about__text"
        >We want to help you thrive! Whether you are just looking for someone to talk to, or are struggling with a mental wellness issue we’re here to help. Our highly talented therapists can help you with a range of issues including relationships, sex, PTSD, depression, social anxiety, or even just caring for yourself more.</div>
      </div>
    </div>
    <div class="b-container b-padding">
      <div class="b-can-help">
        <div class="b-can-help__title">WE CAN HELP YOU WITH</div>
        <boxes-help></boxes-help>
      </div>
    </div>
    <div class="b-container b-padding">
      <div class="b-know-discr">
        <div class="b-know-img"></div>
        <div class="b-know-content">
          <div class="b-know-content__title">YOU SHOULD ALSO KNOW</div>
          <div class="b-know-content__text">
            MDD affects more than 16.1 million American adults, or about 6.7%of the U.S. population age 18 and older in a given year. We at
            <span>
              <logo></logo>
            </span>
            can help you.
          </div>
          <div class="b-know-content__btn">GET HELP NOW</div>
        </div>
      </div>
    </div>
    <div class="b-container-contact">
      <div class="b-container">
        <div class="b-contact b-relative">
          <div class="b-contact-content">
            <div class="b-contact-content__titleBlock">CONTACT US</div>
            <div class="b-contact-content__titleText">Ready. Set. Smile</div>
            <div
              class="b-contact-content__text"
            >Take the free online assessment to see if you are a candidate and get started on your journey.</div>
            <div class="b-contact-content__btn">GET HELP NOW</div>
          </div>
          <div class="b-contact-img"></div>
        </div>
      </div>
    </div>
    <div class="b-container">
      <div class="b-info">
        <div class="b-info-img"></div>
        <div class="b-info-info">
          <div class="b-info-blocks">
            <div class="b-info-block">
              <div class="b-info-block__title">SOME INFO</div>
              <div
                class="b-info-block__row"
              >Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula.</div>
            </div>
            <div class="b-info-block">
              <div class="b-info-block__title">ENFOLD HEALTH</div>
              <div class="b-info-block__row">Main Street 1, Olcott Buffalo, United States</div>
              <div class="b-info-block__contact">
                <div class="b-info-block__row">+555 283 784 333</div>
                <p class="b-info-block__row">
                  <a href="office@enfold-health.com">office@enfold-health.com</a>
                </p>
              </div>
            </div>
            <div class="b-info-block">
              <div class="b-info-block__title">OFFICE HOURS</div>
              <div class="b-info-block__row">Mo-Fr: 8:00-19:00</div>
              <div class="b-info-block__row">Sa: 8:00-14:00</div>
              <div class="b-info-block__row">Su: closed</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="b-container-footer">
      <div class="b-container b-padding">
        <div class="b-footer">
          <div class="b-footer__copy">
            &copy;
            <span>Copyright - ThriveTalk 2017</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import logo from "./components/logo.vue"
import us from "./components/us.vue"
import navigation from "./components/navigation.vue"
import boxesHelp from "./components/boxes.vue"

export default {

  name: 'App',
  components: {
    logo,
    us,
    navigation,
    boxesHelp
  },
  methods: {
    changeClass(first, second) {
      document.querySelector(`.b-helping__${first}`).classList.add("b-orange")
      document.querySelector(`.b-helping__${second}`).classList.remove("b-orange")
    }
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}

.b-container {
  max-width: 1440px;
  margin: 0 auto;
}
.b-padding {
  padding-left: 10px;
  padding-right: 10px;
}
.b-relative {
  position: relative;
}
.b-orange {
  background: #f9b640;
  color: white;
}
.b-header {
  min-height: 200px;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  align-items: center;

  @media (min-width: 1440px) {
    & {
      flex-direction: row;
      min-height: 50px;
    }
  }
}
.b-img {
  display: none;

  @media (min-width: 768px) {
    & {
      display: block;
      height: 100%;
      width: 100%;
      background-image: url("./assets/images/helping.png");
      background-position: right top;
      background-repeat: no-repeat;
      background-size: contain;
      position: absolute;
      top: -8px;
    }
  }
  @media (min-width: 1440px) {
    background-size: initial;
  }
}
.b-helping {
  margin-top: 60px;
  color: #22356f;
  position: relative;
  z-index: 1;

  &__content {
    display: flex;
    align-items: center;
    flex-direction: column;
  }
  &__title {
    margin-top: 15px;
    font-size: 28px;
    line-height: 53px;
    letter-spacing: -0.035em;
    text-align: center;
  }
  &__text {
    margin-top: 15px;
    font-size: 24px;
    line-height: 42px;
    text-align: center;
  }
  &__boxBtn {
    margin-top: 15px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  &__who,
  &__what {
    padding: 5px 10px;
  }
  @media (min-width: 1440px) {
    & {
      padding: 164px 0 77px;
    }
    &__content {
      align-items: flex-start;
      max-width: 477px;
    }
    &__title {
      font-size: 48px;
    }
    &__text {
      text-align: left;
    }
    &__boxBtn {
      max-width: 477px;
      margin-top: 63px;
      justify-content: start;
    }
    &__who {
      margin-right: 38px;
    }
    &__who,
    &__what {
      padding: 10px 30px;
    }
  }
}
.b-container-why {
  background: #62d0df;
  padding: 15px;

  @media (min-width: 1440px) {
    padding: 0;
  }
}
.b-why {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  color: white;

  &__title {
    font-size: 36px;
    line-height: 27px;
    letter-spacing: -0.006em;
  }
  &__text {
    font-size: 24px;
    line-height: 35px;
    margin-top: 73px;
    max-width: 555px;
  }
  &__img {
    display: none;
  }
  @media (min-width: 1440px) {
    & {
      padding: 151px 180px 97px 0;
      align-items: flex-start;
    }
    &__title {
      padding-left: 32px;
    }
    &__text {
      text-align: justify;
    }
    &__img {
      display: inline-block;
      width: 100%;
      height: 100%;
      background-image: url("./assets/images/why.png");
      background-position: right top;
      background-repeat: no-repeat;
      position: absolute;
      top: 0;
      right: 0;
    }
  }
}
.b-about {
  color: #22356f;

  &__title {
    font-size: 16px;
    line-height: 23px;
    letter-spacing: 0.06em;
  }
  &__text {
    font-size: 24px;
    line-height: 33.75px;
    margin-top: 15px;
    text-align: center;
  }

  @media (min-width: 1440px) {
    & {
      display: flex;
      padding: 69px 0 82px;
    }
    &__title {
      margin-right: 200px;
      display: flex;
      align-items: flex-start;
    }
    &__text {
      max-width: 550px;
      text-align: justify;
      display: flex;
      padding-top: 57px;
    }
  }
}
.b-can-help {
  display: flex;
  flex-direction: column;
  align-items: center;

  &__title {
    font-size: 16px;
    line-height: 19px;
    letter-spacing: 0.06em;
    color: rgba(34, 53, 111, 0.5);
  }
}
.b-know-discr {
  display: flex;
  justify-content: space-between;
}
.b-know-img {
  display: none;

  @media (min-width: 768px) {
    & {
      display: inline-block;
      min-width: 280px;
      min-height: 400px;
      background-image: url("./assets/images/know.png");
      background-position: left top;
      background-repeat: no-repeat;
      background-size: contain;
    }
  }
  @media (min-width: 1440px) {
    & {
      min-width: 480px;
      min-height: 800px;
    }
  }
}
.b-know-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  color: #22356f;
  text-align: justify;

  &__title {
    font-size: 16px;
    line-height: 12px;
    letter-spacing: 0.06em;
  }
  &__text {
    font-size: 36px;
    line-height: 53px;
    letter-spacing: -0.01em;
    margin-top: 10px;
  }
  &__text span {
    margin-right: 5px;
  }
  &__btn {
    font-size: 16px;
    line-height: 23px;
    letter-spacing: 0.1em;
    color: #fab63e;
    margin-top: 10px;
    padding: 10px 30px;
    text-align: center;
  }
  &__btn:hover {
    color: white;
    background: #fab63e;
  }
  @media (min-width: 768px) {
    & {
      padding: 0 10px;
    }
  }
  @media (min-width: 1024px) {
    justify-content: center;
  }
  @media (min-width: 1440px) {
    & {
      padding: 103px 106px;
      max-width: 676px;
      align-items: flex-start;
      text-align: left;
    }
    &__title {
      font-size: 26px;
    }
    &__text {
      margin-top: 225px;
    }
    &__btn {
      margin-top: 152px;
      text-align: left;
      padding: 0;
      display: inline-block;
    }
    &__btn {
      padding: 20px 40px;
      font-size: 26px;
      font-weight: 700;
    }
  }
}
.b-container-contact {
  background: #22356f;
}
.b-contact {
  display: flex;
  justify-content: space-between;
}
.b-contact-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: #ffffff;
  text-align: center;

  &__titleBlock {
    font-size: 16px;
    line-height: 12px;
    letter-spacing: 0.06em;
  }
  &__titleText {
    font-size: 44px;
    line-height: 94px;
    letter-spacing: -0.01em;
  }
  &__text {
    font-size: 36px;
    line-height: 53px;
    letter-spacing: -0.005em;
  }
  &__btn {
    margin-top: 55px;
    font-size: 16px;
    line-height: 23px;
    letter-spacing: 0.1em;
    padding: 10px 30px;
    color: #62d0df;
  }
  &__btn:hover {
    color: white;
    background: #fab63e;
  }
  @media (min-width: 1440px) {
    & {
      padding: 103px 201px 42px 205px;
      text-align: left;
      align-items: flex-start;
      justify-content: space-between;
    }
    &__titleText {
      margin-top: 230px;
      font-size: 64px;
    }
    &__text {
      margin-top: 75px;
    }
    &__btn {
      margin-top: 65px;
    }
  }
}
.b-contact-img {
  display: none;

  @media (min-width: 1440px) {
    display: block;
    background-image: url("./assets/images/contact.png");
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    min-width: 480px;
    min-height: 100%;
  }
}
.b-info {
  display: flex;
  justify-content: center;
  padding-top: 20px;

  @media (min-width: 1440px) {
    & {
      justify-content: space-between;
      padding-top: 0;
    }
  }
}
.b-info-img {
  display: none;
  @media (min-width: 1440px) {
    & {
      display: block;
      background-image: url("./assets/images/info.png");
      background-repeat: no-repeat;
      background-size: cover;
      background-position: left top;
      width: 570px;
      min-height: 100%;
    }
  }
}
.b-info-blocks {
  display: flex;
  flex-direction: column;
  @media (min-width: 1440px) {
    & {
      flex-direction: row;
      justify-content: space-between;
      padding: 98px 40px 74px 68px;
      width: 635px;
    }
  }
}
.b-info-block {
  display: flex;
  flex-direction: column;
  align-items: center;

  &:not(:last-child) {
    margin-bottom: 20px;
  }
  &__title {
    margin-top: 10px;
    font-size: 14px;
    line-height: 11px;
    letter-spacing: -0.006em;
    font-weight: 700;
    color: #22356f;
    text-align: center;
  }
  &__row {
    margin-top: 10px;
    font-size: 14px;
    line-height: 23px;
    letter-spacing: -0.006em;
    color: rgba(34, 53, 111, 0.5);
  }
  &__row a {
    text-decoration: none;
  }
  &__contact {
    margin-top: 37px;
    text-align: center;
  }
  @media (min-width: 1440px) {
    & {
      max-width: 165px;
      align-items: flex-start;
    }
    &__title {
      margin-bottom: 52px;
    }
    &__row {
      text-align: left;
    }
    &__contact {
      text-align: left;
    }
  }
}
.b-container-footer {
  background: #62d0df;
}
.b-footer {
  color: white;
  display: flex;
  justify-content: flex-start;
  padding: 32px 0 26px;
}
</style>
