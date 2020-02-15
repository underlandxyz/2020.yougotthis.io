<template>
  <div id='page' class='w'>
    <h1 id="title">Inclusion Programme</h1>
    <p>As part of our commitment to running an accessible, inclusive and safe conference for everyone we are working with <a href="https://mykindof.tech">My Kind of Tech</a>.</p>
    <p>Our inclusion programme includes tickets for those in under-represented groups in tech. This includes, but isn't limited to: LGBTQIA+ people, people of colour, women, non-binary people, and those with disabilities. Our application process should only take 5 minutes, and doesn't ask you to disclose any information which is sensitive. If you have questions about it, <a href="mailto:ygt@underland.events">please get in touch with us via email</a>.</p>
    <div class="scholarships">
      <div class="types">
        <div class="type">
          <h2>Ticket-only scholarships</h2>
          <p>We are committed to give away at least 20% of our available tickets to this kind of scholarship.</p>
          <ul>
            <li>Completely free ticket</li>
            <li>You still have to cover the cost of travel (and accommodation if there is any).</li>
            <li>Applications for our third round of ticket-only scholarships are now open.</li>
          </ul>
        </div>
        <div class="type">
          <h2>Full scholarships</h2>
          <p>Applications for full scholarships have now closed.</p>
        </div>
      </div>
      <!-- <a href="https://airtable.com/shr1hfyrzRBEHjZgs" class="apply" target="_blank">Apply for a ticket-only scholarship before 31st December 2019</a> -->
    </div>
    <ul class="other">
      <li>
        <h2>Code of Conduct</h2>
        <p>Our event has a <n-link to='conduct'>Code of Conduct</n-link> which will be enforced. All attendees, sponsors, team members and vendors will be expected to abide by it.</p>
      </li>
      <li>
        <h2>Venue</h2>
        <p>Our venue is accessible to those with wheelchairs and those who would prefer to not use stairs. We also have gender neutral toilets available.</p>
      </li>
      <li>
        <h2>Closed Captioning</h2>
        <p>We've arranged for talks to be transcribed live, which will be displayed alongside the speaker's slides. The transcripts will also be available after the event and as Closed Captions within the YouTube video recordings.</p>
      </li>
      <li>
        <h2>Speakers</h2>
        <p>Speakers are selected by blind review of their proposed talks without any identifying information. They are being paid for their time.</p>
      </li>
      <li>
        <h2>Food</h2>
        <p>All food will be vegan, with good options for anyone who has more specific dietary requirements. This will extend throughout the event.</p>
      </li>
      <li>
        <h2>Care Team</h2>
        <p>We have a dedicated care team who exist to support any attendees who need support during the event. This is provided by My Kind Of Tech.</p>
      </li>
      <li>
        <h2>Pronoun Awareness</h2>
        <p>It's important to us that people use each others' preferred pronouns. As well as pronoun badges, we'll be making sure the audience is made aware of what pronouns are in the opening talk.</p>
      </li>
      <li>
        <h2>Childcare</h2>
        <p>We will provide stipends for childcare to scholarship recipients. We can provide these in-advance to ensure attendees are cost neutral.</p>
      </li>
    </ul>
    <p>The Underland and My Kind Of Tech teams hope this will make the event comfortable for everyone. If there's something more you think we could be doing, <a href="mailto:ygt@underland.events">please get in touch</a>.</p>
  </div>
</template>

<style lang="scss" scoped>
#page {
  margin-top: 2em;
  margin-bottom: 2em;
  * {
    margin-bottom: 1rem;
  }
  ul {
    margin-left: 1.25em;
  }
}
.scholarships {
  background: var(--secondary-light);
  padding: 1em;
  margin-top: 2em;
  margin-bottom: 2em;
  .types {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 2em;
    margin-bottom: 0 !important;
  }
  h3 {
    text-align: center;
  }
}

#page ul.other {
  list-style-type: none;
  padding-left: 0;
  margin-left: 0;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 4em;
  margin-top: 4em;
  margin-bottom: 4em;
  li {
    margin-left: 0;
    margin-bottom: 0;
    h2 {
      color: var(--theme);
    }
    p {
      margin-bottom: 0;
    }
  }
  + p {
    margin-bottom: 4em;
  }
}

.apply {
  background: var(--theme-dark);
  display: block;
  text-align: center;
  padding: 0.75em;
  color: white;
  text-decoration: none;
  margin-bottom: 0 !important;
}

@media screen and (max-width: 600px) {
  .scholarships .types,
  #page ul.other {
    grid-template-columns: 1fr;
    grid-gap: 1em;
  }
}
</style>
