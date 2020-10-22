<template>
<div class="home">
    <m-table :tableData="tableData" :tableColumns="tableColumns" />
</div>
</template>

<script>
// @ is an alias to /src
import mTable from '@/components/mTable.vue'

export default {
    name: 'Home',
    components: {
        'm-table': mTable
    },
    data() {
        return {
            tableData: [],
            tableColumns: [{
                fixed: true,
                prop: 'date',
                label: '日期',
                width: 150
            }, {

                prop: 'name',
                label: '姓名',
                width: 120
            }]
        }
    },
}
</script>
