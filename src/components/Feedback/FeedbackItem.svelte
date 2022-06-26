<script lang="ts">
  import Card from '../common/Card.svelte';

  export let item;
  const handleDelete = (itemId: number) => {
    console.log(itemId);
  };
</script>

<Card>
  <div class="num-display">
    {item.rating}
  </div>
  <div class="close" on:click={() => handleDelete(item.id)}>X</div>
  <p class="text-display">
    {item.text}
  </p>
</Card>

<style>
  .num-display {
    position: absolute;
    top: -10px;
    left: -10px;
    width: 30px;
    height: 30px;
    background-color: #ff6a95;
    color: #fff;
    border: 1px #eee solid;
    border-radius: 50%;
    padding: 10px;
    text-align: center;
    font-size: 19px;
  }
  .close {
    position: absolute;
    top: 10px;
    right: 20px;
    cursor: pointer;
  }

  .text-display {
    font-size: 1.5em;
    text-align: center;
    margin-bottom: 10px;
  }
</style>
