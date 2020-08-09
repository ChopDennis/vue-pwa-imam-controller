<template>
    <div id="imam-controller-nav">
        <b-container>
            <b-navbar
                    toggleable="lg"
                    type="dark"
            >
                <b-navbar-brand
                        to="/"
                >
                    <span class="mx-1">今時科技</span>
                </b-navbar-brand>
                <b-navbar-toggle target="nav-collapse" />
                <b-collapse
                        id="nav-collapse"
                        is-nav
                >
                    <b-navbar-nav>
                        <b-nav-item
                                to="/config"
                                class="my-3 text-center"
                        >
                            Config
                        </b-nav-item>
                    </b-navbar-nav>
                </b-collapse>
            </b-navbar>
        </b-container>
    </div>
</template>

<script>
    export default {
        name: "TheHeader",
    }
</script>

<style scoped>
    #imam-controller-nav {
        background-color: #42b983;
    }

    #nav-collapse {
        background-color: #42b983;
        z-index: 99;
    }

    @media screen and (max-width: 991px) {
        #nav-collapse {
            margin: 0 -2rem;
        }
    }

    @media screen and (min-width: 992px) {
        #nav-collapse {
            height: 0;
        }
    }

    a {
        color: white !important;
        letter-spacing: 1px;
    }
</style>