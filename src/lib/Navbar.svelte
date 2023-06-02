<script>
    import {navigate} from "svelte-routing";

    var goto;

    function assignRoute(route) {
        goto = route
    }

    function go() {
        navigate(goto)
    }

    function hideOffcanvasAndNavigate(route) {
        const offcanvasElement = document.getElementById('offcanvasDarkNavbar');
        const offcanvasInstance = bootstrap.Offcanvas.getInstance(offcanvasElement);
        offcanvasInstance.hide()
        assignRoute(route)
        setTimeout(go, 400);
    }
</script>

<main>
    <nav class="navbar navbar-dark bg-dark fixed-top">
        <div class="container-fluid">
            <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas"
                    data-bs-target="#offcanvasDarkNavbar" aria-controls="offcanvasDarkNavbar">
                <span class="navbar-toggler-icon"></span>
            </button>
            <a class="navbar-brand">FourGuysProduction</a>
            <div class="offcanvas offcanvas-start text-bg-dark" tabindex="-1" id="offcanvasDarkNavbar"
                 aria-labelledby="offcanvasDarkNavbarLabel">
                <div class="offcanvas-header">
                    <h5 class="offcanvas-title" id="offcanvasDarkNavbarLabel">FourGuysProduction</h5>
                    <button type="button" class="btn-close btn-close-white" data-bs-dismiss="offcanvas"
                            aria-label="Close"></button>
                </div>
                <div class="offcanvas-body">
                    <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
                        <li class="nav-item">
                            <a class="nav-link" on:click={() => hideOffcanvasAndNavigate('/')}
                               href="javascript:void(0)">Home</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" on:click={() => hideOffcanvasAndNavigate('/work')}
                               href="javascript:void(0)">Work</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" on:click={() => hideOffcanvasAndNavigate('/about')}
                               href="javascript:void(0)">About</a>
                        </li>
                        <li class="nav-item dropdown">
                            <a class="nav-link dropdown-toggle" role="button" data-bs-toggle="dropdown"
                               aria-expanded="false">
                                Members
                            </a>
                            <ul class="dropdown-menu dropdown-menu-dark">
                                <li><a class="dropdown-item   "
                                       on:click={() => hideOffcanvasAndNavigate('/TorlapSonprathed')}
                                       href="javascript:void(0)">TorlapSonprathed</a></li>
                                <li><a class="dropdown-item"
                                       on:click={() => hideOffcanvasAndNavigate('/ChayatornOunpat')}
                                       href="javascript:void(0)">ChayatornOunpat</a></li>
                                <li><a class="dropdown-item"
                                       on:click={() => hideOffcanvasAndNavigate('/PiyoungkulSawang')}
                                       href="javascript:void(0)">PiyoungkulSawang</a></li>
                                <li><a class="dropdown-item"
                                       on:click={() => hideOffcanvasAndNavigate('/JirawatSapthawarakul')}
                                       href="javascript:void(0)">JirawatSapthawarakul</a></li>
                            </ul>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </nav>
</main>

<style>

</style>
