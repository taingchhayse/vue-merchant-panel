<template>
  <div class="dashboard-container">
    <section class="content container-fluid">
    <div class="row">
      <div class="col-xs-6">
        <div class="box">
          <div class="box-body">
            <div id="defaultDataTable_wrapper" class="dataTables_wrapper form-inline dt-bootstrap no-footer"><div class="row"><div class="col-sm-6"></div><div class="col-sm-6"></div></div><div class="row"><div class="col-sm-12"><div class="dataTables_scroll"><div class="dataTables_scrollHead" style="overflow: hidden; position: relative; border: 0px; width: 100%;"><div class="dataTables_scrollHeadInner" style="box-sizing: content-box; width: 573.5px; padding-right: 0px;"><table class="table table-bordered table-hover nowrap dataTable no-footer" role="grid" style="margin-left: 0px; width: 573.5px;"><thead>
              <tr role="row"><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 181.859px;">支付编码/PayTypeId</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 44.1328px;">别名</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 44.1328px;">货币</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 74.4141px;">费率(%)</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 82.1719px;">充值限额</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 43.7891px;">状态</th></tr></thead></table></div></div><div class="dataTables_scrollBody" style="position: relative; overflow: auto; width: 100%;"><table id="defaultDataTable" class="table table-bordered table-hover nowrap dataTable no-footer" role="grid"><thead>
              <tr role="row" style="height: 0px;"><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 181.859px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">支付编码/PayTypeId</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 44.1328px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">别名</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 44.1328px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">货币</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 74.4141px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">费率(%)</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 82.1719px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">充值限额</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 43.7891px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">状态</div></th></tr></thead>
              
              <tbody><tr class="odd"><td valign="top" colspan="6" class="dataTables_empty">表中数据为空</td></tr></tbody>
            </table></div></div><div id="defaultDataTable_processing" class="dataTables_processing panel panel-default" style="display: none;">处理中...</div></div></div><div class="row"><div class="col-sm-5"></div><div class="col-sm-7"></div></div></div>
            * 别名仅供参考，具体用途与作用以开户文档描述为准，或咨询客服人员
          </div>
        </div>
      </div>
    </div>
  </section>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'

export default {
  name: 'RechargeCodeAndRate',
  computed: {
    ...mapGetters([
      'name'
    ])
  }
}
</script>

<style lang="scss" scoped>
// .dashboard {
//   &-container {
//     margin: 30px;
//   }
//   &-text {
//     font-size: 30px;
//     line-height: 46px;
//   }
// }
.box-body{
    border-top-left-radius: 0;
    border-top-right-radius: 0;
    border-bottom-right-radius: 3px;
    border-bottom-left-radius: 3px;
    padding: 10px;
}
</style>
