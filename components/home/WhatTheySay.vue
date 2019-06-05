<template>
  <div id="what-they-say" class='w'>
    <div class="tiles">
      <div class="tile text secondary">
        <h2>2019 Highlights</h2>
      </div>
      <div class="tile img">
        <img src="~/assets/highlights/1.jpg" alt="">
      </div>
      <div class="tile vid">
        <iframe src="https://www.youtube.com/embed/xdizooyxRjk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="tile img">
        <img src="~/assets/highlights/2.jpg" alt="">
      </div>
      <div class="tile tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">I went to <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> today and genuinely had such an amazing time. Met some lovely people, sat in on talks on subjects I resonated with such as anxiety, imposter syndrome and self-care</p>&mdash; Myles Adamson (@adamson_myles) <a href="https://twitter.com/adamson_myles/status/1086701099137011712?ref_src=twsrc%5Etfw">January 19, 2019</a></blockquote>
      </div>
      <div class="tile img">
        <img src="~/assets/highlights/3.jpg" alt="">
      </div>
      <div class="tile img sn">
        <img src="~/assets/highlights/violet-sn.jpg" alt="">
      </div>
      <div class="tile tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr"><a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> was a phenomenally inspiring experience! Best technology event I&#39;ve been to, hands down. Big thanks to everyone at <a href="https://twitter.com/underlandxyz?ref_src=twsrc%5Etfw">@underlandxyz</a> for organising, can&#39;t wait for next year!</p>&mdash; Chris McIntyre (@cgmcintyr) <a href="https://twitter.com/cgmcintyr/status/1086721634353012738?ref_src=twsrc%5Etfw">January 19, 2019</a></blockquote>
      </div>
      <div class="tile vid">
        <iframe src="https://www.youtube.com/embed/oXAGFrj-D4M" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="tile img">
        <img src="~/assets/highlights/4.jpg" alt="">
      </div>
      <div class="tile tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">It was a pleasure to be part of the <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> at the weekend. Someone said it was the &#39;single most positive atmosphere at a tech conference I&#39;ve been to&#39;. This is amazing feedback and we hope the event will help early career <a href="https://twitter.com/hashtag/developers?src=hash&amp;ref_src=twsrc%5Etfw">#developers</a> achieve a happy, healthy work life. <a href="https://t.co/nY0K2tDfux">pic.twitter.com/nY0K2tDfux</a></p>&mdash; AND Digital (@AND_Digital) <a href="https://twitter.com/AND_Digital/status/1087315386985525248?ref_src=twsrc%5Etfw">January 21, 2019</a></blockquote>
      </div>
      <div class="tile img">
        <img src="~/assets/highlights/5.jpg" alt="">
      </div>
      <div class="tile vid">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/eE9DyaxO8Z0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
      <div class="tile img">
        <img src="~/assets/highlights/6.jpg" alt="">
      </div>
      <div class="tile tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">I had a fantastic time at <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> today. Thank you for organising this wonderful event, <a href="https://twitter.com/underlandxyz?ref_src=twsrc%5Etfw">@underlandxyz</a>. I wish it spreads to more parts of the world. We need to have these difficult and awkward but rewarding conversations in the tech industry. 💖</p>&mdash; ✨Shubheksha✨ (@ScribblingOn) <a href="https://twitter.com/ScribblingOn/status/1086730786282393600?ref_src=twsrc%5Etfw">January 19, 2019</a></blockquote>
      </div>
      <div class="tile img sn">
        <img src="~/assets/highlights/paula-sn.jpg" alt="">
      </div>
      <div class="tile tweet">
        <blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">I had intended to leave the <a href="https://twitter.com/hashtag/YouGotThisConf?src=hash&amp;ref_src=twsrc%5Etfw">#YouGotThisConf</a> earlier in the afternoon to go work on my stem cells but the conference was SO GOOD I ended up staying all day! Thanks <a href="https://twitter.com/underlandxyz?ref_src=twsrc%5Etfw">@underlandxyz</a> for the great kickstart to 2019. Feeling motivated and inspired (eventho I&#39;m not a programmer) 😋🥰🌠 <a href="https://t.co/jZm3Yi63ww">pic.twitter.com/jZm3Yi63ww</a></p>&mdash; 🎆🌈Rachel Konichiwakitty🌟🎉 (@konichiwakitty) <a href="https://twitter.com/konichiwakitty/status/1086698393559318530?ref_src=twsrc%5Etfw">January 19, 2019</a></blockquote>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  head () {
    return { 
      script: [
        { async: true, src: 'https://platform.twitter.com/widgets.js', charset: 'utf-8' }
      ]
    }
  },
}
</script>


<style lang="scss" scoped>
.tiles {
  columns: 2;
  margin-top: 4em;
  margin-bottom: 2em;
}
.tile {
  margin-bottom: 1em;
  &.text {
    padding: 1em;
    border-radius: 4px;
    &.secondary {
      background: var(--secondary);
      color: white;
    }
  }
  &.img {
    img {
      width: 100%;
      border-radius: 4px;
      display: block;
    }
    &.sn {
      border: 1px solid #e8e8e8;
      padding: 1em;
      border-radius: 4px;
    }
  }
  &.vid {
    iframe {
      width: 100%;
      height: 230px;
    }
  }
  blockquote {
    display: inline-block;
    border: 1px solid #e8e8e8;
    padding: 1em;
    border-radius: 4px;
  }
}
</style>