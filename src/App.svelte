<script lang="ts">
  import FeedbackList from './components/Feedback/FeedbackList.svelte';

  let feedbacks = [
    {
      id: 1,
      rating: 10,
      text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam eius corporis, nam error dolorem modi adipisci molestiae doloribus est? Expedita magni provident asperiores architecto eaque ea saepe optio natus tempore!',
    },
    {
      id: 2,
      rating: 9,
      text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam eius corporis, nam error dolorem modi adipisci molestiae doloribus est? Expedita magni provident asperiores architecto eaque ea saepe optio natus tempore!',
    },
    {
      id: 3,
      rating: 8,
      text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquam eius corporis, nam error dolorem modi adipisci molestiae doloribus est? Expedita magni provident asperiores architecto eaque ea saepe optio natus tempore!',
    },
  ];
</script>

<main>
  <FeedbackList {feedbacks} />
</main>
