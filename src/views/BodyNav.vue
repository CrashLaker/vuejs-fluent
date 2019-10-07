<template>
    <div id="bodynav">
        <ul style="margin-top:0;" role="navigation" id="sidenav-small" class="nav side-navigation side-navigation-small theme-default">
            <button type="button" class="close" data-dismiss="side-navigation" aria-label="close">
                <i class="glyph glyph-cancel"></i>
            </button>
            <li class="active side-nav-c2" v-for="(list, key, topicid) in content" :key="topicid"> 
                <a data-toggle="collapse" data-parent="#sidenav-small" href="#father-john-misty" aria-expanded="true" aria-controls="#father-john-misty">
                    {{ key }}
                </a>
                <!--<ul class="nav collapse in" id="father-john-misty">-->
                <ul class="nav" id="father-john-misty">
                    <li v-for="(item, itemid) in list" :key="itemid">
                        <a href="#sidenav-small">
                            {{ item }}
                        </a>
                    </li>
                </ul>
            </li>
        </ul>
    </div>
</template>


<script>
export default {
    data(){
        return {
            content: {
                'Introdução': [
                    'Contexto',
                    'Resumo Executivo'
                ],
                'RAGs': [
                    'Infra Geral',
                    'Aplicações',
                    'Oracle/SQL Core',
                    'AWS EC2/RDS'
                ],
                'VMWare': [
                    'Cluster HA - 1 Host',
                    'Hosts Status',
                    'VMs Status',
                    'TOP VMs CPU/MEM' 
                ],
                'Storage': [
                    'Highend',
                    'Midrange',
                    'Fileshare',
                    'AllFlash'
                ],
                'Backup': [
                    'Janela',
                    'Volume',
                    'Fitas',
                    'Licença'
                ],
                'Oracle': [
                    'Disk'
                ],
                'AWS': [
                    'EC2',
                    'RDS'
                ],
                'Network': [
                    'Usage'
                ]
            }
        }
    }
}
</script>