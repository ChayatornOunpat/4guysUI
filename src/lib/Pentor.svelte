<script>
    import Navbar from "./Navbar.svelte";
    import Footer from "./Footer.svelte";
</script>

<div style="height: 100%; display: flex; flex-direction: column">
    <Navbar></Navbar>
    <div class="container col-xxl-8 px-4 py-5 row-content" style="flex-grow: 1">
        <div class="row flex-lg-row-reverse align-items-center g-5 py-5">
            <div class="col-10 col-sm-8 col-lg-6">
                <img src="http://127.0.0.1:8000/img/pentor" class="d-block mx-lg-auto img-fluid rounded border border-secondary"
                     alt="Bootstrap Themes"
                     width="700"
                     height="500" loading="lazy">
            </div>
            <div class="col-lg-6">
                <h1 class="display-5 fw-bold lh-1 mb-3">Torlap Sonprathed</h1>
                <p class="lead">Quickly design and customize responsive mobile-first sites with Bootstrap, the
                    world’s
                    most popular front-end open source toolkit, featuring Sass variables and mixins, responsive grid
                    system, extensive prebuilt components, and powerful JavaScript plugins.</p>
            </div>
        </div>
    </div>
    <Footer></Footer>
</div>


<style>

</style>