<template>
  <div id='page' class='w'>
    <h1 id="title">Schedule</h1>
    <div class="list">
      <div class="item" v-for="slot in schedule" :key="slot[0]" :class="{content: slot[2]}">
        <h2>{{slot[0]}} <span class="speaker" v-if='slot[2]'> - {{slot[3]}}</span></h2>
        <p>{{slot[1]}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      schedule: [
        ['09:00', 'Registration opens', false],
        ['10:00', 'Welcome talk', false],
        ['10:30', 'Keynote - It\'s not your job to love your job', true, 'Keziyah Lewis'],
        ['11:00', 'Talk - Learning to invest in your future', true, 'Matthew Gilliard'],
        ['11:30', 'Comfort break', false],
        ['12:00', 'Talk - How to find your perfect mentor', true, 'Amina Adewusi'],
        ['12:30', 'Talk - So good they can\'t ignore you! 😎', true, 'Gargi Sharma'],
        ['13:00', 'Lunch break', false],
        ['14:00', 'Keynote - Level Up: Developing Developers', true, 'Melinda Seckington'],
        ['14:30', 'Talk - 0 to 100 Real Quick: making your first days count', true, 'Nathaniel Okenwa'],
        ['15:00', 'Comfort break', false],
        ['15:30', 'Talk - Company Culture, Performance Reviews & You', true, 'Ruth Lee'],
        ['16:00', 'Talk - Unions Got This: organising the tech trade', true, 'Dan Parkes'],
        ['16:30', 'Short comfort break', false],
        ['16:45', 'Keynote - Real talk about when to walk away', true, 'Amy Dickens'],
        ['17:15', 'Farewell talk', false],
        ['17:45', 'Networking (dry event)', false],
        ['19:00', 'Event ends', false]
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
#page {
  margin-top: 2em;
  margin-bottom: 2em;
}
.list {
  margin-bottom: 4em;
}
.item {
  border: 1px solid rgba(0, 0, 0, 0.2);
  padding: 1em;
  margin-top: 1em;
  margin-bottom: 2em;
  box-shadow: 0 3px 5px -1px rgba(0,0,0,.2), 0 6px 10px 0 rgba(0,0,0,.14), 0 1px 18px 0 rgba(0,0,0,.12);
  &.content {
    background: var(--secondary-light)
  }
}
@media screen and (max-width: 800px) {
  h2 {
    font-size: 1.25em;
  }
}
</style>
