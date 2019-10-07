<template>
    <div id="ppt">
        <Breadcrumb />
        <div class="container">
            <div class="row">
                <div class="col-md-4">
                    <BodyNav />
                </div>
                <div class="col-md-8">
                    <Body />
                </div>
            </div>
        </div>
    </div>
</template>


<script>
import Breadcrumb from "@/views/Breadcrumb.vue";
//import Body from "@/views/Body.vue";
import BodyNav from "@/views/BodyNav.vue";

export default {
    components: {
        Breadcrumb,
        BodyNav
    }
}
</script>