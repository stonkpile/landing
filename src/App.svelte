<script lang="ts">
import Topbar from './components/Topbar.svelte'
import Logotype from './components/Logotype.svelte'
import Navigation from './components/Navigation.svelte'
import Footer from './components/Footer.svelte'
import { Button } from '@stonkpile/ui-kit'

export let name: string
</script>

<section class="hero is-large">
  <div class="hero-head">
    <Topbar>
      <Logotype></Logotype>
      <Navigation></Navigation>
    </Topbar>
  </div>

  <div class="hero-body">
    <div class="container is-max-desktop has-text-centered">
      <h1 class="title is-1 is-spaced">HELLO! Track all of your assets in one place</h1>
      <h2 class="subtitle is-4">Lorem ipsum dolor sit amet consectetur adipisicing elit.<br />Necessitatibus explicabo soluta.</h2>
    </div>
    
    <div class="buttons are-medium is-centered">
      <Button type="is-primary">Sign up</Button>
      <Button>Sign in</Button>
    </div>
  </div>
</section>

<section class="hero is-medium is-light">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns">
        <div class="column">
          <h1 class="title is-4">Stocks</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>

        <div class="column">
          <h1 class="title is-4">Crypto</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>

        <div class="column">
          <h1 class="title is-4">Gold & Silver</h1>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="hero is-medium is-primary">
  <div class="hero-body">
    <div class="container is-max-desktop">
      <div class="columns">
        <div class="column is-6">
          <h1 class="title is-1 is-spaced">Keep track</h1>
          <p class="subtitle is-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Labore fuga possimus dolorem quia, perferendis id illum inventore atque! Quos laudantium non magni sequi deleniti quaerat sed eveniet odio doloribus praesentium</p>
          <p class="subtitle is-5">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Labore fuga possimus dolorem quia, perferendis id illum inventore atque</p>
        </div>

        <div class="column is-5 is-offset-1">
          <img src="/track.svg" />
        </div>
      </div>
    </div>
  </div>
</section>

<Footer></Footer>

<style lang="scss" global>
  $primary:  #fd746c;
  @import "bulma/bulma";

  .buttons {
    margin-top: 2.5rem;
  }

  :root {
    --noise:url(data:image/png;base64,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);
  }

  .hero.is-light {
    background: var(--noise), linear-gradient(127deg,whitesmoke, #f5f5f5); 
  }

  .hero.is-primary {
    background: var(--noise), linear-gradient(127deg, #fd746c, #ff9068); 
  }
</style>
