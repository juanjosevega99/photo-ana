<script>
  import Profile from "./Profile.svelte";
  import Stories from "./Stories.svelte";
  import Footer from "./Footer.svelte";
</script>

<style>
  .TimeLine {
    padding: 4em 0 0 0;
  }
</style>

<div class="Sidebar">
  <div class="Sidebar-container">
    <Profile />
    <Stories />
    <Footer />
  </div>
</div>
