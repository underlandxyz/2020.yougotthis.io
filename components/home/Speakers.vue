<template>
  <div id='speakers' class='w'>
    <h2>Here's who's speaking...</h2>
    <div class="list">
      <Speaker v-for='speaker in speakers' :key='speaker.name' :speaker='speaker' />
    </div>
  </div>
</template>

<script>
import Speaker from '~/components/home/Speaker';

export default {
  data() {
    return {
      speakers: [
        {
          name: 'Amy Dickens',
          twitter: 'RedRoxProjects',
          avatar: require('~/assets/speakers/amy-dickens.png'),
          color: '#5457BE',
          title: 'Never stop stopping - real talk about when to walk away',
          desc: [
            'When you start your first job there is a ton of learning to be done, not just about the job itself but the office space & social norms between your colleagues. It can be exciting, challenging & at times overwhelming.',
            'But what happens if the excitement wears off all too quickly & suddenly you’re not sure you want the job any longer?',
            'In this talk we will take an honest look at what happens when your new job becomes your worst job. Including tools to help you recognize the signs of this happening & what you can do to establish your own boundaries & rules about when to walk away.'
          ]
        },
        {
          avatar: require('~/assets/speakers/question.png'),
          title: 'More speakers announced soon',
          color: '#FF004A'
        }
      ]
    }
  },
  components: {
    Speaker
  }
}
</script>

<style lang="scss" scoped>
#speakers {
  border-bottom: 1px solid var(--secondary-light);
  border-top: 1px solid var(--secondary-light);
  margin-bottom: 4em;
  padding-top: 4em;
  padding-bottom: 4em;
  h2 {
    text-align: center;
    margin-bottom: 2em;
  }
  h3 {
    text-align: center;
    margin-top: 1em;
  }
}
.list {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 2em;
}
@media screen and (max-width: 1000px) {
  .list {
    grid-template-columns: 1fr;
  }
}
</style>