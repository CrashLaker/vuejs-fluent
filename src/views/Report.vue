<template>
    <div id="report">
        <div class="container">
            <ol class="breadcrumb">
                <li><a href="#">Report</a></li>
                <li><a href="#">Setembro 2019</a></li>
                <li class="active">TOP VMs CPU/MEM</li>
            </ol>
            <div class="h4">
                Report TOP VMs CPU/MEM > 70% Setembro 2019
            </div> 
            <ol class="list-items">
                <li class="list-items-row">
                    <div aria-expanded="false">
                        <div class="row">
                            <div class="col-md-2">
                                <strong>ID</strong>
                            </div>
                            <div class="col-md-6">
                                Col1
                            </div>
                            <div class="col-md-4">
                                Col2
                            </div>
                            <div class="col-md-4">
                                Col3
                            </div>
                            <div class="col-md-4">
                                Col4
                            </div>
                            <div class="col-md-4 text-right">
                                Col5
                            </div>
                        </div>
                    </div>
                </li>
                <li v-for="(item,itemid) in list" :key="itemid" class="list-items-row">
                    <div data-toggle="collapse" 
                         aria-expanded="false" 
                         :data-target="'#list-item-line-' + item">
                        <div class="row">
                            <div class="col-md-2">
                                <i class="glyph glyph-add"></i>
                                <i class="glyph glyph-remove"></i>
                                <strong>{{ item }}</strong>
                            </div>
                            <div class="col-md-6">
                                <a>Link</a>
                            </div>
                            <div class="col-md-4">
                                Text
                            </div>
                            <div class="col-md-4">
                                Text
                            </div>
                            <div class="col-md-4">
                                Text
                            </div>
                            <div class="col-md-4 text-right">
                                <a>Link</a>
                            </div>
                        </div>
                    </div>
            
                    <div class="collapse" :id="'list-item-line-' + item">
                        <div class="row">
                            <div class="col-md-18 col-md-offset-2">
                                Lorem ipsum dolor sit amet.
                            </div>
                            <div class="col-md-4 text-right">
                                <button class="btn btn-primary btn-sm">Button</button>
                            </div>
                        </div>
                    </div>
                </li>
            </ol>
        </div>
    </div>
</template>


<script>
export default {
    data(){
        return {
            list: [
                1,
                2,
                3,
                4,
                5,
                6,
                7,
                8,
                9,
                10
            ]
        }
    }
}
</script>

<style>

</style>