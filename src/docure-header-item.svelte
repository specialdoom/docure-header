<svelte:options tag="docure-header-item" />

<slot />

<style>
  :host {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    height: 64px;
    min-width: 5%;
    color: #4392f1;
    cursor: pointer;
  }

  :host([isright]) {
    float: right;
  }

  ::slotted(a) {
    text-decoration: none;
    color: #4392f1;
    height: 100%;
    width: 100%;
    display: flex;
    padding: 0 16px;
    justify-content: center;
    align-items: center;
  }

  ::slotted(a:hover) {
    text-decoration: underline;
  }

  ::slotted(a[aria-current]) {
    background: #4392f1;
    color: #fff;
  }

  ::slotted(a[aria-current]:hover) {
    text-decoration: none;
  }
</style>
