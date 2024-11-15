<script>
  import {Button} from "$lib";
  import {page} from '$app/stores';

  $effect(() => {
    console.log('effect', $page.url.pathname);
  })
</script>

<p>
  <a href="/">Home</a>
  <Button url="/test/page1">Shallow 1</Button>
  <Button url="/test/page2">Shallow 2</Button>
  <Button url="/test/page3">Shallow 3</Button>
</p>

<style>
  p {
    display: flex;
    gap: 1em;
  }
</style>
