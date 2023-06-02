<script>
    import {Link} from "svelte-routing";
</script>


<div class="shadow-lg bg-dark align-items-center justify-content-center custom-rounded-top">
    <div class="mb-5">
        <ul class="nav justify-content-center mt-5 mb-4">
            <li class="nav-item">
                <Link to="/" class="nav-link px-2 text-muted">Home</Link>
            </li>
            <li class="nav-item">
                <Link to="/about" class="nav-link px-2 text-muted">About</Link>
            </li>
            <li class="nav-item">
                <Link to="/work" class="nav-link px-2 text-muted">Work</Link>
            </li>
            <li class="nav-item">
                <Link to="/PiyoungkulSawang" class="nav-link px-2 text-muted">PiyoungkulSawang</Link>
            </li>
            <li class="nav-item">
                <Link to="/TorlapSonprathed" class="nav-link px-2 text-muted">TorlapSonprathed</Link>
            </li>
            <li class="nav-item">
                <Link to="/JirawatSapthawarakul" class="nav-link px-2 text-muted">JirawatSapthawarakul</Link>
            </li>
            <li class="nav-item">
                <Link to="/ChayatornOunpat" class="nav-link px-2 text-muted">ChayatornOunpat</Link>
            </li>
        </ul>
        <p class="text-center text-light">FourGuysProduction</p>
    </div>
</div>


<style>
    .custom-rounded-top {
        border-top-left-radius: 2rem;
        border-top-right-radius: 2rem;
    }
</style>