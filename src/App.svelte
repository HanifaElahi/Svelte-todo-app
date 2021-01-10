<script>
  import Header from "./components/Header.svelte";
  import List from "./components/List.svelte";
</script>

<style>
  .container {
    width: 700px;
    height: 525px;
    padding: 120px 500px 120px 500px;
    background:purple;
  }

  :global(.container *) {
    font-family: "Quicksand", sans-serif;
  }
</style>

<div class="container">
  <Header />
  <List />
</div>
