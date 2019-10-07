<template>
    <div id="nav">
        <nav class="navbar navbar-default">
            <div class="navbar-global theme-default">
                <div class="container">
                    <div class="navbar-header">
                        <button
                            type="button"
                            class="navbar-toggle collapsed"
                            data-toggle="collapse"
                            data-target="#bs-example-navbar-collapse-1"
                        >
                            <span class="sr-only">Toggle navigation</span>
                            <i class="glyph glyph-hamburger"></i>
                        </button>

                        <router-link to="/" class="navbar-brand">
                            <img src="@/../public/logo.png" alt="BTG Capacity Planning" height="48" />
                        </router-link>
                    </div>
                    <div style="margin-top:15px;" class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
                        <ul class="nav navbar-nav">
                            <li class="dropdown">
                                <router-link
                                    to="/"
                                    class="dropdown-toggle"
                                    data-toggle="dropdown"
                                    role="button"
                                    aria-expanded="false">
                                    Home
                                </router-link>
                            </li>

                            <li class="dropdown">
                                <router-link to="/ppt">
                                    PPT
                                </router-link>
                            </li>

                            <li class="dropdown">
                                <router-link to="/report">
                                    Report
                                </router-link>
                            </li>

                            <li class="dropdown">
                                <router-link to="/about">
                                    About
                                </router-link>
                            </li>

                            <li class="dropdown">
                                <a
                                    href="#!"
                                    class="dropdown-toggle"
                                    data-toggle="dropdown"
                                    role="button"
                                    aria-expanded="false"
                                >
                                    Tools
                                    <i class="glyph glyph-chevron-down-2"></i>
                                </a>
                                <ul class="dropdown-menu" role="menu">
                                    <li>
                                        <router-link to="/tools/icons">
                                            Icons
                                        </router-link>
                                    </li>
                                </ul>
                            </li>
                        </ul>
                        <form class="navbar-form navbar-right" role="search">
                            <div class="form-group">
                                <input type="search" class="form-control" placeholder="Search" />
                            </div>
                            <button type="submit" class="btn btn-default"></button>
                        </form>
                    </div>
                </div>
            </div>
        </nav>
    </div>
</template>


<script>
export default {
    name: "Navbar",
    data() {
        return {};
    }
};
</script>

<style>
#nav {
    height: 70px;
    border-bottom:1px solid#cecece;
}
</style>