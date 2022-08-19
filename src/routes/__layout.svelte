<script context="module">
  import { storyblokInit, apiPlugin } from "@storyblok/svelte";
  import Feature from "../components/Feature.svelte";
  import Grid from "../components/Grid.svelte";
  import Page from "../components/Page.svelte";
  import Teaser from "../components/Teaser.svelte";

  storyblokInit({
    accessToken: "1HabIcxFOnH2q9Mw0U1wPAtt",
    use: [apiPlugin],
    components: {
      feature: Feature,
      grid: Grid,
      page: Page,
      teaser: Teaser,
    },
  });
</script>

<script>
  import "../app.css";
</script>

<main>
  <slot />
</main>
