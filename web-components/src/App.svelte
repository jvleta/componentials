<script>
  import Card from "./Card.svelte";
  import BoilerPlate from "./BoilerPlate.svelte";
  import AccordionItem from "./AccordionItem.svelte";
  export let name = "Mom";
</script>

<main>
  <BoilerPlate  year="2022" company_name="Jimmy Leta">
    <h1>Hello {name}!!!</h1>
    <Card card_title="My Card Title" card_desc="Lorem ipsum dolor…" />
  </BoilerPlate>
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
