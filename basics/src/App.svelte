<script>
  import { Router, Route } from 'svelte-routing';
  import Page from "./Page.svelte";
</script>

<main>
<Router>
  <Route component={Page}></Route>
  <Route path=":index" let:params>
      <Page noteIndex={params.index}/>
  </Route>
</Router>
  
</main>
