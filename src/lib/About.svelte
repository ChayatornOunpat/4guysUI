<script>
    import Navbar from "./Navbar.svelte";
    import Footer from "./Footer.svelte";
</script>

<div style="height: 100%; display: flex; flex-direction: column">
    <Navbar></Navbar>
    <img class="img-fluid img-max" src="http://127.0.0.1:8000/img/homemain">
    <div class="px-4 py-5 my-5 text-center" style="flex-grow: 1">
        <h1 class="display-5 fw-bold">About us</h1>
        <div class="col-lg-6 mx-auto">
            <p class="lead mb-4">just four idiots filming stuff </p>
        </div>
    </div>
    <Footer></Footer>
</div>

<style>
    .img-max {
        width: 100%;
    }
</style>