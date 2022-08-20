<svelte:options tag="boiler-plate" />
<script>
  export let year, company_name;
</script>

<div class="content">
  <slot></slot>
</div>

<footer class="footer">
  &copy; {year} {company_name}
</footer>

<style>
  .content {
    min-height: calc(100vh - 70px);
  }
  .footer {
    padding-top: 20px;
    border-top-color: black;
    border-top: 2px;
    border-top-style: solid;
    text-align: center;
  }
</style>
