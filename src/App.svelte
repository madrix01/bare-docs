<script>
    import Router from './routes/index.svelte'
</script>

<main>
    <h1>Bare Cli</h1>
    <p class="subtitle">Manage all your boilerplate and generate boilerplate files from your commandline</p>
    <a href="https://github.com/madrix01/Bare" target="_blank"><img src="https://img.shields.io/badge/Github-%20madrix01%2FBare-blue" alt="GitHub"></a>
    <!-- <Link to="install">install</Link> -->
    <div class="nav">
        <a href="/">Home</a>
        <a href="/install">Install</a>
        <a href="/use">Use</a>
        <a href="/commands">Commands</a>
        <a href="/recipe">Recipe</a>
    </div>
    <div class="pages">
        <Router />
    </div>
</main>

<style>
    main {
        text-align: center;
        max-width: 240px;
        margin: 0 auto;
        padding-bottom: 20px;
    }
    .pages {
        width: 50%;
        margin: 0 auto;
        text-align: left;
    }
    .subtitle{
        text-align: center;
        color : #00AFFF;
        font-size: large;
    }
    
    
    :global(body) {
        background-color: rgb(30, 35, 51);
        color: white;
        font-family: 'Fira Code', monospace;
    }

    h1 {
        color: #ffffff;
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
    }
    a {
        text-decoration: none;
        color: white;
    }

    .nav {
        margin: 0 auto;
        width: 50%;
        display: flex;
        justify-content: space-evenly;
    }

    ::-webkit-scrollbar {
        display: none;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>