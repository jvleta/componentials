<svelte:options tag="my-card" />
<script>
  export let title, description;
</script>

<main>
  <div class="card-container">
    <div class="card">
      <div class="card-body">
        <div class="row">
          <div class="card-title">
            <h2>{title}</h2>
          </div>
        </div>
        <p>
          {description}
        </p>
        <button>Launch</button>
      </div>
    </div>
  </div>
</main>

<style>
  .card {
    max-width: 350px;
    border-radius: 5px;
    box-shadow: 0 4px 6px 0 #00000033;
    padding: 0 0 10px 0;
  }

  .card-body {
    padding: 5px 10px;
  }

  .card-body p {
    color: #575757;
    margin-bottom: 20px;
    font-size: 14px;
  }

  .card-container {
    padding: 20px;
  }
</style>
