<svelte:options tag="docure-header" />

<script>
  export let logosource = "";
</script>

<div class="docure-header">
  <div class="docure-header-logo">
    <img src={logosource} alt="Logo" />
  </div>
  <div class="docure-header-nav">
    <slot />
  </div>
</div>

<style>
  .docure-header {
    box-sizing: border-box;
    width: 100%;
    height: 64px;
    background-color: #fff;
    display: flex;
    align-items: center;
    padding: 0 32px;
    box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
  }
  .docure-header-logo {
    width: 10%;
  }

  .docure-header-nav {
    width: 90%;
  }
  .docure-header-logo img {
    width: 110px;
    height: 50px;
    margin-right: 16px;
  }

  @media only screen and (max-width: 700px) {
    .docure-header-logo {
      width: 20%;
    }

    .docure-header-nav {
      width: 80%;
    }
  }
</style>
