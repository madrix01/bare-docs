<script>
    import Router from './routes/index.svelte'
</script>

<main>
    <h1>Bare Cli</h1>
    <a href="https://github.com/bare-cli/Bare" target="_blank"><img src="https://img.shields.io/badge/bare--cli-bare-blue?style=flat-square&logo=github" alt="GitHub"></a>
    <a href="https://www.npmjs.com/package/barego" target="_blank"><img src="https://img.shields.io/npm/dt/barego?style=flat-square&logo=npm" alt="npm"></a>
    <a href="https://github.com/bare-cli/Bare" target="_blank"><img src="https://img.shields.io/github/stars/bare-cli/Bare?logo=github&style=flat-square" alt="GitHub"></a>
    <a href="https://www.npmjs.com/package/barego" target="_blank"><img src="https://img.shields.io/npm/v/barego?style=flat-square&logo=npm" alt="npm version"></a>
    <p class="subtitle">Manage all your boilerplate and generate boilerplate files from your commandline</p>
    <p class="comments">Please write your review <a href="https://github.com/madrix01/bare/issues/new" target="_blank"><u>Here</u></a></p>
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
    
    .comments {
        font-size: 25px;
        color: blue;
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