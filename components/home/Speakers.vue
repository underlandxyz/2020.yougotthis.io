<template>
  <div id="speakers" class="w">
    <h2>Here's who's speaking...</h2>
    <div class="list">
      <Speaker v-for="speaker in speakers" :key="speaker.name" :speaker="speaker" />
    </div>
  </div>
</template>

<script>
import Speaker from '~/components/home/Speaker'

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
          bio:
            'Amy is a Developer Community Manager for Pusher - a company that helps developers build realtime features into their projects through hosted APIs. Amy’s career has traversed the worlds of music, audio and tech - finally finding their jam in community management. Having worked many jobs (over 15 to date) Amy is well versed in knowing when it is time to look for something new - a feeling that is familiar for many of us and that they will cover in their (exclusive to You Got This) talk.'
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
            'In this talk, we will cover exactly what you should say when reaching out to someone you don’t know, whether in-person or online. We will explore how to interact with your mentor to understand and meet their needs, so that you can create a sustainable symbiotic relationship.'
          ],
          bio:
            'Amina is an Associate Software Engineer at the Guardian News & Media in London. She taught herself how to code whilst looking after a young baby and juggling a full-time job. She is passionate about encouraging under-represented groups into tech and is proof that it’s possible to become an engineer without spending a penny. She is an international speaker who seeks to represent the voice of new developers in the software engineering industry.'
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
          bio:
            'Dan is the Chair of the West Midlands Regional Group of Game Workers Unite UK. He’s also an Audio Engineer at Pixel Toys and has worked in the games industry for 6 years across audio, data and design disciplines.'
        },
        {
          name: 'Nathaniel Okenwa',
          twitter: 'chatterboxCoder',
          avatar: require('~/assets/speakers/nathaniel-okenwa.png'),
          color: '#FF0045',
          title: '0 to 100 Real Quick - Making your First Days Count',
          desc: [
            'Hooray! You’ve landed your first full-time tech job, but what comes next? The first few months can be daunting and it is easy to feel like you don’t belong. In this talk, we look at some useful strategies to help you navigate your rookie year.',
            'Last year, I started my first full-time role as a Developer Evangelist. Speaking with fellow newbies, I realised how similar our experiences were. Over the past 12 months, I have collected useful learnings to guide others through this early phase of their careers. Whether you’re new in tech and looking for your first role, a new hire just starting or a manager onboarding juniors, this talk will provide you with a checklist of actionable practices to ace your first year.'
          ],
          bio:
            "Nathaniel is a Developer Evangelist at Twilio working to create magical moments for developers with their products. He is a die hard fan of JavaScript, sports, superheroes and mixed martial arts. His life goals are to have Batman's brains, Deadpool's humour, T'Challa's fashion sense, Killmonger's Wokeness, and Thanos' determination! He serves the Javascript community in the UK and the rest of Europe."
        },
        {
          name: 'Gargi Sharma',
          twitter: 'gawwrgi',
          avatar: require('~/assets/speakers/gargi-sharma.png'),
          color: '#00BF8E',
          title: "So good they can't ignore you! 😎",
          desc: [
            'You are good at your job, are polite and deadline oriented. Your long-term professional goals are well-defined, and you work toward them consistently.',
            'But working hard is sometimes not enough. People around you need to see and value your work.',
            'This talk will cover hard-work, visibility, the myth of meritocracy, and what we owe one another once we are “successful”.'
          ],
          bio:
            'Gargi is a systems engineer at Tarides, who really cares about building teams with psychological safety.  Gargi is really passionate about teaching, systems programming and Modern Art. In the past, Gargi attended the Recurse Center, volunteered at AddisCoder, worked as a software engineer at Bloomberg LP, and wrote some code for the Linux Kernel.'
        },
        {
          name: 'Ruth Lee',
          twitter: 'yoursruthlessly',
          avatar: require('~/assets/speakers/ruth-lee.png'),
          color: '#5457BE',
          title: 'Company Culture, Performance Reviews & You',
          desc: [
            `"Culture fit". The dreaded phrase we all love to hear in our rejection letters, but culture's more than just being a cis white dude. In this talk I'll discuss engineering culture, particularly around approaches to risk and maturity of processes in companies of different sizes. This talk is aimed at helping junior engineers understand how this culture impacts performance reviews and how to adapt to flourish in different company environments.`,
            `You'll get the low down on engineering team culture from a business perspective. We'll cover what culture is (approach to risk) and isn’t (free snacks). Company and team culture archetypes (startup vs. mature) and suggest which suit different career and comfort levels.`,
            `We'll also look at how company culture impacts your career especially the effect on performance reviews and feedback. How you should account for this in your own self assessment, and strategies for assessing stated versus actual culture.`
          ],
          bio:
            "Ruth is an Engineering Manager for the Site Reliability Team at Splunk. She's been a Linux engineer for almost a decade during which time she's developed an unhealthy obsession with the topic of time in computing. Outside of work you can find her on a mountain, the sea, or at the gym powerlifting."
        },
        {
          name: 'Keziyah Lewis',
          twitter: 'KeziyahL',
          avatar: require('~/assets/speakers/keziyah-lewis.png'),
          color: '#FF0045',
          title: "It's not your job to love your job",
          desc: [
            'Tech workers are under enormous pressure to put our jobs above anything else in our lives. Startup culture encourages self sacrifice and overwork in order to complete the company’s mission. As early career devs, it’s easy to feel that we should be grateful to have a job in this industry, especially when you have a decent salary and perks, and your boss is constantly reminding you that you’re part of a “family” that is “changing the world”.',
            'Loving or appreciating your job isn’t a problem on its own. But you’re not obligated to do it. In fact, I’d argue that the pressure to love your job can be dangerous. Using examples from my personal experience and from the tech industry as a whole, I’ll talk about how unconditional job love is used to exploit or mistreat tech workers.',
            'You’ll leave this talk with a better understanding of techniques employers use to mask workplace issues, how to view your workplace more critically, how to spot cultural red flags, and how to advocate for yourself and your colleagues.'
          ],
          bio:
            'Keziyah Lewis is a Black and queer web developer, designer, and digital nomad. She curates Juniors in Tech, a newsletter for early career technologists. Keziyah is passionate about eliminating barriers to entering tech, making the industry more diverse and just, and making tech companies better places to work.'
        },
        {
          name: 'Melinda Seckington',
          twitter: 'mseckington',
          avatar: require('~/assets/speakers/melinda-seckington.png'),
          color: '#FF6F00',
          title: 'Level Up: Developing Developers',
          desc: [
            'As video games have become more and more complex, game designers put way more time into creating environments where players are engaged and willing to put the time and effort into learning and mastering these skills.',
            'We can learn a lot from how games are designed to make the internal developer experiences better, since it’s a similar type of environment we want to create: an environment where people can learn and master skills. We should make it easier for developers to understand what options are available to them, allow them to make time for learning and provide structures and processes for them to develop the skills that they want and need for future roles.',
            'This talk will look at how you can help level up your team by using competencies and career development frameworks, what types of processes you can introduce to support personal development and how developers should be using opportunities like these to get a better understanding of what skills they should focus on.'
          ],
          bio:
            'Melinda Seckington is a Technical Manager at FutureLearn, the social learning platform offering free and paid-for online courses and degrees from leading universities and organisations worldwide. She speaks at international technology conferences and writes for MissGeeky, a blog about all things geeky and girly. When she’s not busy with events or blogging, you can find Melinda curled up on her couch with a good book or video game.'
        },
        {
          name: 'Matthew Gilliard',
          twitter: 'MaximumGilliard',
          avatar: require('~/assets/speakers/matthew-gilliard.png'),
          color: '#FF6F00',
          title: 'Learning to Invest in Your Future',
          desc: [
            'When change is the only constant, learning is the only future-proof skill. But deadlines, rules and the pressure to ship working code can stop us from learning effectively. To do that we need to give ourselves permission to switch mindset; to try new things, to have fun and to embrace our curiosity.',
            'In this talk, using examples from the pioneers of programming education in the 1960s through to the present day, Matthew will show some effective techniques for developing new programming skills. You’ll see how learning how to learn can benefit you through your whole career, and how valuable it can be to share what you’ve learned with others. As well as making your programming more fun and more interesting, you’ll find out how cultivating your learning can benefit your employer and set you up for success.'
          ],
          bio:
            'Matthew is a Developer Evangelist for Twilio, a company that is helping developers to fuel the future of communication with APIs. He loves spending time with the programming community at conferences, meetups and hackathons, helping developers to discover their superpowers.'
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
  border-top: 1px solid var(--secondary-light);
  margin-bottom: 4em;
  padding-top: 4em;
  padding-bottom: 2em;
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