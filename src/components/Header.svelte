<script>
  import { items } from "../stores";

  $: itemCount = $items.length;
  $: completedItemCount = $items.filter((item) => item.complete).length;
</script>

<style>
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 25px 25px;
    color: #eeeeee;
    font-weight: bold;
    font-size: 1.5em;
    background: rgba(0, 0, 0, 0.6);
  }
</style>

<div class="header">
  <div>My To-Do List</div>
  <span> {completedItemCount}/{itemCount} </span>
</div>
