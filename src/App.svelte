<script>
    import Router from './routes/index.svelte'
</script>

<main>
    <h1>Bare Cli</h1>
    <p class="subtitle">Manage all your boilerplate and generate boilerplate files from your commandline</p>
    <!-- <Link to="install">install</Link> -->
    <div class="nav">
        <a href="/">Home</a>
        <a href="/install">Install</a>
        <a href="/use">Use</a>
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
        color: white
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

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>