<script>
    import {Router, Route} from 'svelte-routing'
    import Home from '../Home.svelte'
    import Install from '../Install.svelte'
    import Usage from '../Usage.svelte'
    import Commands from '../Commands.svelte'    
    import Recipe from '../Recipe.svelte';
    export let url = '';

</script>

<Router {url}>
    <div>
        <Route path="install" component={Install} />
        <Route path="/" component={Home} />
        <Route path="use" component={Usage} />
        <Route path="commands" component={Commands}/>
        <Route path="recipe" component={Recipe}/>
    </div>
</Router>