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
          ],
          bio: 'Amy is a Developer Community Manager for Pusher - a company that helps developers build realtime features into their projects through hosted APIs. Amy’s career has traversed the worlds of music, audio and tech - finally finding their jam in community management. Having worked many jobs (over 15 to date) Amy is well versed in knowing when it is time to look for something new - a feeling that is familiar for many of us and that they will cover in their (exclusive to You Got This) talk.'
        },
        {
          name: 'Amina Adewusi',
          twitter: 'a_adewusi',
          avatar: require('~/assets/speakers/amina-adewusi.png'),
          color: '#00BF8E',
          title: 'How to find your perfect mentor, when you don’t know how',
          desc: [
            'Achieving your goals, whether to teach yourself how to code, get your first developer job or level up in your career are very likely to require support from a mentor.',
            'Identifying and connecting with good mentors ensures that the time you spend trying to achieve your goals is both efficient and effective. Mentors can open doors to more knowledge, job opportunities and support you mentally and emotionally. ',
            'In this talk, we will cover exactly what you should say when reaching out to someone you don’t know, whether in-person or online. We will explore how to interact with your mentor to understand and meet their needs, so that you can create a sustainable symbiotic relationship.',
          ],
          bio: 'Amina is an Associate Software Engineer at the Guardian News & Media in London. She taught herself how to code whilst looking after a young baby and juggling a full-time job. She is passionate about encouraging under-represented groups into tech and is proof that it’s possible to become an engineer without spending a penny. She is an international speaker who seeks to represent the voice of new developers in the software engineering industry.'
        },
        {
          name: 'Dan Parkes',
          twitter: 'dancparkes',
          avatar: require('~/assets/speakers/dan-parkes.png'),
          color: '#FF6F00',
          title: 'Unions Got This - Organising the Tech Trade',
          desc: [
            'Unions don’t usually come up in history class. If they do, they’re normally accompanied by talk of miners and Thatcherism. But we’re not taught what unions actually do for the modern, nine-to-five worker. That’s where this talk comes in.',
            'This will be a whistle-stop tour of what unionism means in today’s world of tech. We’ll briefly cover what a union is, the various shapes and sizes they take and what they can do for you, using the recently formed Game Workers Unite UK branch of the IWGB as an example.',
            'We’ll also touch upon the happenings across the pond at Kickstarter and Vox Media as well as how the international movements of Game Workers Unite and the Tech Workers Coalition are bringing unionism into tech industries.'
          ],
          bio: 'Dan is the Chair of the West Midlands Regional Group of Game Workers Unite UK. He’s also an Audio Engineer at Pixel Toys and has worked in the games industry for 6 years across audio, data and design disciplines.'
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
  grid-gap: 2.5em;
}
@media screen and (max-width: 1000px) {
  .list {
    grid-template-columns: 1fr;
  }
}
</style>