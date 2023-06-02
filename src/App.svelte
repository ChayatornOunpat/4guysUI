<script>
    import { Router, Route } from 'svelte-routing';
    import Home from "./lib/Home.svelte";
    import About from "./lib/About.svelte";
    import Me from "./lib/Me.svelte";
    import Mickey from "./lib/Mickey.svelte";
    import Pentor from "./lib/Pentor.svelte";
    import Tonhom from "./lib/Tonhom.svelte";
    import Work from "./lib/Work.svelte";
</script>

<svelte:head>
    <link href='https://fonts.googleapis.com/css?family=Noto Sans' rel='stylesheet'>
</svelte:head>

<Router>
    <Route path="/" component={Home} />
    <Route path="/about" component={About} />
    <Route path="/work" component={Work} />
    <Route path="/PiyoungkulSawang" component={Tonhom} />
    <Route path="/TorlapSonprathed" component={Pentor} />
    <Route path="/JirawatSapthawarakul" component={Mickey} />
    <Route path="/ChayatornOunpat" component={Me} />
</Router>

<style>

</style>
