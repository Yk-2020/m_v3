<template>
<div class="table">
    <el-table :data="tableData" style="width:100%" height="250">
        <el-table-column v-for="(v,i) in tableColumns" :key="i" :fixed="v.fixed" :prop="v.prop" :label="v.label" :width="v.width">
        </el-table-column>
    </el-table>
</div>
</template>

<script>
export default {
    name: 'Table',
    props: ['tableData', 'tableColumns']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style lang="scss" scoped>

</style>
