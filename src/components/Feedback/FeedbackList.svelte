<script lang="ts">
  import FeedbackItem from './FeedbackItem.svelte';

  export let feedbacks = [];
</script>

{#each feedbacks as fb (fb.id)}
  <FeedbackItem item={fb} on:delete-feedback />
{/each}
