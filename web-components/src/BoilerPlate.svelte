<svelte:options tag="boiler-plate" />

<script>
  export let app_name, year, company_name;
</script>
<header class="header"><h1>{app_name}</h1></header>
<div class="content">
  <slot />
</div>

<footer class="footer">
  &copy; {year}
  {company_name}
</footer>

<style>
  .header {
    grid-column: 1 / 4;
    font-size: x-large;
    border-bottom-color: black;
    border-bottom: 2px;
    border-bottom-style: solid;
    padding-top: 10px;
    padding-bottom: 10px;
  }
  .content {
    min-height: calc(100vh - 70px);
  }
  .footer {
    padding-top: 10px;
    padding-bottom: 10px;
    border-top-color: black;
    border-top: 2px;
    border-top-style: solid;
    text-align: center;
  }
</style>
