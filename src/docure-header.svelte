<svelte:options tag="docure-header" />

<div class="docure-header">
  <slot />
</div>

<style>
  :host {
    display: block;
    box-sizing: border-box;
    width: 100%;
    height: 64px;
    background-color: #fff;
    padding: 0 32px;
    box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
  }
</style>
