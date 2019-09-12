<template>
  <div>
    <div class="speaker">
      <div class="main">
        <img :src="speaker.avatar" alt="">
        <div class="meta">
          <p class='title'>{{ speaker.title }}</p>
          <p v-if='speaker.name'>{{ speaker.name }} <a v-if='speaker.twitter' :href="'https://twitter.com/' + speaker.twitter" target="_blank">(@{{ speaker.twitter }})</a></p>
          <small 
            v-if='speaker.desc' 
            @click="showDetails = !showDetails"
            :style="{ color: speaker.color }">{{ moreText }}</small>
        </div>
      </div>
      <div class="details" v-if='showDetails'>
        <p v-for='p in speaker.desc' :key='p'>{{ p }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showDetails: false
    }
  },
  computed: {
    moreText() {
      return this.showDetails ? 'Hide details' : 'More details'
    }
  },
  props: ['speaker']
}
</script>

<style lang="scss" scoped>
.speaker {
  display: inline-block;
}
.main {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  img {
    width: 100px;
    height: 100px;
    margin-right: 1em;
  }
  p.title {
    font-weight: bold;
    margin-bottom: 0.5em;
  }
  small {
    display: inline-block;
    margin-top: 0.5em;
    cursor: pointer;
  }
}
.details {
  p {
    margin-top: 1em;
  }
}
@media screen and (max-width: 1000px) {
  .main img {
    width: 200px;
    height: 200px;
    margin-right: 2em;
  }
}
@media screen and (max-width: 800px) {
  .speaker {
    display: block;
  }
  .main {
    flex-direction: column;
    text-align: center;
    img {
      margin: 0 0 1em;
    }
  }
  .details {
    text-align: center;
  }
}
</style>