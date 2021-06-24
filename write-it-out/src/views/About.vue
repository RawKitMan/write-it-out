<template>
  <b-container>
    <div class="about">
      <h1 id="about-title">About CJ and Rhonda</h1>
      <BImg
        :src="require('../assets/images/ThisIsUs.jpg')"
        fluid
        thumbnail
        alt="Rhonda and CJ"
        id="aboutImage"
      ></BImg>
      <div>
        <p>
          We are CJ and Rhonda. We are married with a joined family that we
          adore. We work very hard to provide, but lately felt a stagnation in
          our lives. We believed we were not truly living in a healthy way,
          mentally and physically. Upon coming to this realization, we have
          implemented many changes in order to achieve the following goals:
        </p>
      </div>
      <ul id="goals">
        <li>Achieve physical health via weight loss and increased mobility</li>
        <li>
          Control our finances so we can live within our means and save/pay off
          debt
        </li>
        <li>Take a two week vacation to Canada</li>
      </ul>
      <div>
        <p>
          These goals sound simple but life long changes can be very difficult
          to maintain. This site will be used to document how well/poorly we are
          doing in achieving our goals as well as how it is affecting us.
          Welcome to the journey.
        </p>
      </div>
    </div>
  </b-container>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import { BImg, BContainer } from "bootstrap-vue";
@Component<About>({
  components: {
    BImg,
    BContainer,
  },
})
export default class About extends Vue {
  private ourImage = "../assets/images/ThisIsUs.jpg";
}
</script>

<style lang="scss" scoped>
#goals {
  display: inline-block;
}
#goals li {
  list-style-type: none;
  font-weight: 900;
}
#aboutImage {
  height: 25%;
  width: 25%;
  margin-bottom: 1em;
}
</style>
