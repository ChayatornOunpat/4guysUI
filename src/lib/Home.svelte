<script>
    import Navbar from "./Navbar.svelte";
    import {Link} from "svelte-routing";
    import Footer from "./Footer.svelte";
</script>

<main>
    <Navbar></Navbar>
    <img class="img-fluid img-max" src="http://127.0.0.1:8000/img/homemain">
    <div class="px-4 py-5 my-5 text-center">
        <h1 class="display-5 fw-bold">FourGuysProduction</h1>
        <div class="col-lg-6 mx-auto">
            <p class="lead mb-4">just four idiots filming stuff </p>
            <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
                <Link to="/about" class="btn btn-primary btn-lg px-4 gap-3">More about us</Link>
            </div>
        </div>
    </div>
    <div class="d-grid gap-3 align-items-center justify-content-center">
        <div class="shadow-lg bg-dark custom-rounded">
            <div class="row row-cols-2 g-3 ms-4 me-4 mt-4 mb-4">
                <div class="col">
                    <div class="card">
                        <img src="http://127.0.0.1:8000/img/pentor" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Torlap Sonprathed</h5>
                            <p class="card-text">Our great emperor, drinks coffee from african children</p>
                            <Link to="/TorlapSonprathed" class="btn btn-primary">More</Link>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <img src="http://127.0.0.1:8000/img/me" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Chayatorn Ounpat</h5>
                            <p class="card-text">I can dislocate all my joints when I sleep, its pretty comfy</p>
                            <Link to="/ChayatornOunpat" class="btn btn-primary">More</Link>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <img src="http://127.0.0.1:8000/img/tonhom" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Piyoungkul Sawang</h5>
                            <p class="card-text">drinks milk from african children instead of mont fleur</p>
                            <Link to="/PiyoungkulSawang" class="btn btn-primary">More</Link>
                        </div>
                    </div>
                </div>
                <div class="col">
                    <div class="card">
                        <img src="http://127.0.0.1:8000/img/mickey" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h5 class="card-title">Jirawat Sapthawarakul</h5>
                            <p class="card-text">buy RTX3090 to play solitaire and candy crush</p>
                            <Link to="/JirawatSapthawarakul" class="btn btn-primary">More</Link>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="ms-4 me-4 mt-4 mb-4">
            <div class="card">
                <div class="card-img-top">
                    <video src="http://127.0.0.1:8000/video/reel" class="w-100" controls></video>
                </div>
                <div class="card-body">
                    <h5 class="card-title">Reel</h5>
                    <p class="card-text">slander compilation of all our work</p>
                    <Link to="/work" class="btn btn-primary">More of our work</Link>
                </div>
            </div>
        </div>
        <Footer></Footer>
    </div>
</main>

<style>
    .custom-rounded {
        border-radius: 2rem;
    }

    .custom-rounded-top {
        border-top-left-radius: 2rem;
        border-top-right-radius: 2rem;
    }

    .img-max {
        width: 100%;
    }
</style>