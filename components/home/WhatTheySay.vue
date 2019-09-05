<template>
  <div id="highlights" class='w'>
    <h2>And here's what happened last year...</h2>
    <img src="~/assets/highlights/2019.png" alt="A selection of images from 2019's event">
    <iframe src="https://www.youtube.com/embed/videoseries?list=PLhLrx4Pimiyk3jcO9kDhQtCRDKeRgv5zg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    <div class="tweets">
      <div class="tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">I went to <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> today and genuinely had such an amazing time. Met some lovely people, sat in on talks on subjects I resonated with such as anxiety, imposter syndrome and self-care</p><small>&mdash; Myles Adamson (@adamson_myles) <a href="https://twitter.com/adamson_myles/status/1086701099137011712?ref_src=twsrc%5Etfw">January 19, 2019</a></small></blockquote>
      </div>
      <div class="tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr"><a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> was a phenomenally inspiring experience! Best technology event I&#39;ve been to, hands down. Big thanks to everyone at <a href="https://twitter.com/underlandxyz?ref_src=twsrc%5Etfw">@underlandxyz</a> for organising, can&#39;t wait for next year!</p><small>&mdash; Chris McIntyre (@cgmcintyr) <a href="https://twitter.com/cgmcintyr/status/1086721634353012738?ref_src=twsrc%5Etfw">January 19, 2019</a></small></blockquote>
      </div>
      <div class="tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">It was a pleasure to be part of the <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> at the weekend. Someone said it was the &#39;single most positive atmosphere at a tech conference I&#39;ve been to&#39;. This is amazing feedback and we hope the event will help early career <a href="https://twitter.com/hashtag/developers?src=hash&amp;ref_src=twsrc%5Etfw">#developers</a> achieve a happy, healthy work life. <a href="https://t.co/nY0K2tDfux">pic.twitter.com/nY0K2tDfux</a></p><small>&mdash; AND Digital (@AND_Digital) <a href="https://twitter.com/AND_Digital/status/1087315386985525248?ref_src=twsrc%5Etfw">January 21, 2019</a></small></blockquote>
      </div>
      <div class="tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">I had a fantastic time at <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> today. Thank you for organising this wonderful event, <a href="https://twitter.com/underlandxyz?ref_src=twsrc%5Etfw">@underlandxyz</a>. I wish it spreads to more parts of the world. We need to have these difficult and awkward but rewarding conversations in the tech industry. 💖</p><small>&mdash; ✨Shubheksha✨ (@ScribblingOn) <a href="https://twitter.com/ScribblingOn/status/1086730786282393600?ref_src=twsrc%5Etfw">January 19, 2019</a></small></blockquote>
      </div>
      <div class="tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">I had intended to leave the <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> earlier in the afternoon to go work on my stem cells but the conference was SO GOOD I ended up staying all day! Thanks <a href="https://twitter.com/underlandxyz?ref_src=twsrc%5Etfw">@underlandxyz</a> for the great kickstart to 2019. Feeling motivated and inspired (eventho I&#39;m not a programmer) 😋🥰🌠 <a href="https://t.co/jZm3Yi63ww">pic.twitter.com/jZm3Yi63ww</a></p><small>&mdash; 🎆🌈Rachel Konichiwakitty🌟🎉 (@konichiwakitty) <a href="https://twitter.com/konichiwakitty/status/1086698393559318530?ref_src=twsrc%5Etfw">January 19, 2019</a></small></blockquote>
      </div>
      <a href='https://2019.yougotthis.io/highlights' class="more">
        👉🏻  See more highlights on last year's site
      </a>
    </div>
  </div>
</template>


<style lang="scss" scoped>
#highlights {
  margin-bottom: 4rem;
}
h2 {
  text-align: center;
  margin-bottom: 1rem;
}
img {
  width: 100%;
}
iframe {
  margin-top: 2em;
  width: 100%;
  height: 500px;
}
.tweets {
  columns: 2;
  column-gap: 2em;
  margin-top: 2em;
  .tweet {
    margin-bottom: 2em;
    blockquote {
      display: inline-block;
      border: 1px solid #e8e8e8;
      padding: 1em;
      small {
        display: block;
        margin-top: 1em;
      }
    }
  }
  .more {
    background: var(--secondary);
    color: white;
    padding: 0.75em;
    text-decoration: none;
    display: inline-block;
    font-size: 1.25em;
    width: 100%;
  }
}
@media screen and (max-width: 800px) {
  img {
    display: none;
  }
  .tweets {
    columns: 1;
  }
  iframe {
    height: 54vw;
    margin-top: 0;
  }
}
</style>