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
  display: grid;
  grid-template-columns: 125px auto;
  grid-gap: 1em;
  img {
    width: 100%;
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
.meta {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.details {
  p {
    margin-top: 1em;
  }
}
@media screen and (max-width: 1000px) {
  .speaker {
    width: 100%;
  }
  .main {
    grid-template-columns: 1fr;
    text-align: center;
    img {
      display: block;
      margin: 0 auto;
      width: 60%;
    }
  }
  .details {
    text-align: center;
  }
}
</style>