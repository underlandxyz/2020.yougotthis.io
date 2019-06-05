<template>
  <div id='page' class='w'>
    <h1 id="title">Sponsor You Got This 2020</h1>
    <h2>You Got This is an affordable one-stream conference for early-career developers and their team leaders on skills needed for a happy, healthy work life.</h2>
    <div class="summary">
      <h2>Summary</h2>
      <ul>
        <li>Saturday 18 January 2020</li>
        <li>Birmingham, UK</li>
        <li>300-350 attendees</li>
        <li>Three audiences
          <ul>
            <li>Soon-to-be developers</li>
            <li>Junior devs looking to skill-up</li>
            <li>People managers</li>
          </ul>
        </li>
      </ul>
    </div>
    <div class="why">
      <div class="need">
        <h2>The need</h2>
        <p>There are lots of non-technical skills which early-career developers are never taught. These skills and feelings are rarely spoken about, which we aim to change.</p>
      </div>
      <div class="mission">
        <h2>Our mission</h2>
        <p>By running a conference around these specific themes, we hope to prompt conversations between team members to promote a more happy and healthy work life for all.</p>
      </div>
    </div>
    <div class="adulting">
      <img src="~/assets/site/adulting.png" alt="Adulting.Dev">
      <p>You Got This 2019 is already having an impact in encouraging discussion about these important topics, inspiring a set of event organisers in New York to run their own version of the conference - Adulting.Dev</p>
    </div>
    <div class="sponsorship">
      <h1>Sponsorship packages</h1>
      <ul>
        <li>
          <h3>Bronze - £1,000 + VAT</h3>
          <ul>
            <li>Logo on website</li>
            <li>Tweets of thanks</li>
            <li>Message in event email</li>
            <li>Shout out in opening</li>
            <li>1 ticket to event</li>
          </ul>
        </li>
        <li>
          <h3>Silver - £3,000 + VAT</h3>
          <ul>
            <li>Everything in bronze</li>
            <li>Table and stand in networking area</li>
            <li>5 min lightning talk</li>
            <li>2 tickets to event</li>
          </ul>
        </li>
        <li>
          <h3>Gold - £7,500 + VAT</h3>
          <ul>
            <li>Everything in silver</li>
            <li>Co-branding</li>
            <li>Provide the good coffee</li>
            <li>Branded chill-out area</li>
            <li>4 tickets to event</li>
          </ul>
        </li>
      </ul>
      <div class="more">
        <h2>Additional Sponsorship Opportunities</h2>
        <ul>
          <li>Provide live-captioning - £1,500</li>
          <li>Provide a mid-afternoon snack - £1,500</li>
          <li>Sponsor lunch - £3,000</li>
          <li>Pay for and watermark photography - £1,250</li>
        </ul>
      </div>
      <div class="custom">
        <p>Our sponsorship packages and additional sponsorship opportunities are indications of what we can do, however nothing is set in stone. We’re happy to chat about custom packages or creating custom perks for BASH Festival.</p>
      </div>
    </div>
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
    ul li {
      margin-top: 1em;
    }
  }
}
.summary {
  background: var(--secondary-light);
  padding: 1em;
  margin-top: 2em;
  li:last-child {
    margin-bottom: 0;
  }
}

.why {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 2em;
  margin-top: 2em;
}

.adulting {
  img {
    height: 2.5em;
  }
}

#page .sponsorship {
  margin-top: 2em;
  > ul {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-gap: 2em;
    margin-left: 0;
    padding-left: 0;
    list-style: none;
    li {
      margin-left: 0;
    }
  }
}

#page .custom {
  margin-top: 2em;
  background: var(--theme-light);
  padding: 1em;
  margin-bottom: 2em;
  p {
    margin-bottom: 0;
  }
}
</style>
