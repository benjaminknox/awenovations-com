<script lang="ts">
	import logo from '$lib/assets/logo.svg';
	import avatar from '$lib/assets/avatar.png';
	import Icon from '@awenovations/aura/icon.svelte';

</script>

<div class="wrapper">
  <div class="margin" ></div>
  <image src={logo} />
  <div class="content">
    Awenovations is a software business building focused micro-SaaS applications. Every product is built on a custom design system that ensures speed, consistency, and clarity from concept to release. Awenovations prioritizes simple, effective solutions that scale without unnecessary complexity.
  </div>
  <div class="divider"></div>
  <div class="contact-card">
    <image src={avatar} />
    <div class="links">
      <a class="icon" target="blank" href="https://www.ben-knox.com/"><Icon name="globe" />ben-knox.com</a>
      <a class="icon" target="blank" href="https://www.linkedin.com/in/benjaminknox1"><Icon name="linkedin" />benjaminknox1</a>
      <a class="icon" target="blank" href="https://github.com/benjaminknox"><Icon name="github" />benjaminknox</a>
      <a class="icon" target="blank" href="https://x.com/benjaminpknox"><Icon name="x" />benjaminpknox</a>
    </div>
  </div>
</div>

<style lang="scss">
  .wrapper {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 4.286rem;

    .margin {
      height: 2vw;
    }

    .content {
      width: 28.571rem;
      line-height: 1.5em;
      text-align: justify;
    }

    .divider {
      width: 100%;
      max-width: 17.143rem; 
      min-height: 0.143rem;
      background: var(--aura-secondary-40);
      border-radius: 0.143rem;
    }


    .contact-card {
      display: flex;
      gap: 1rem;

      .links {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;

        a {
          font-style: italic;
          color: var(--aura-secondary-40);
          align-items: self-end;
          gap: 0.5rem;
          display: flex;
          text-decoration: none;
        }
      }
    }

  }
</style>
