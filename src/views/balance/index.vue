<template>
  <div class="dashboard-container">
   <div class="box">
          <div class="box-header">
            <form id="searchForm">
              <div class="row">
                <div class="col-sm-4">
                  <button type="button" class="btn btn-info " onclick="javascript:table.ajax.reload(null, true);"><span class="glyphicon glyphicon-search"></span> 刷新</button>
                </div>
              </div>
            </form>
          </div>
          <div class="box-body">
            <div id="defaultDataTable_wrapper" class="dataTables_wrapper form-inline dt-bootstrap no-footer"><div class="row"><div class="col-sm-6"></div><div class="col-sm-6"></div></div><div class="row"><div class="col-sm-12"><div class="dataTables_scroll"><div class="dataTables_scrollHead" style="overflow: hidden; position: relative; border: 0px; width: 100%;"><div class="dataTables_scrollHeadInner" style="box-sizing: content-box; width: 1197px; padding-right: 0px;"><table class="table table-bordered table-hover nowrap dataTable no-footer" role="grid" style="margin-left: 0px; width: 1197px;"><thead>
              <tr role="row"><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 233.398px;">货币</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 321.016px;">别名</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 321.016px;">可用余额</th><th class="sorting_disabled" rowspan="1" colspan="1" style="width: 252.57px;">冻结中</th></tr></thead></table></div></div><div class="dataTables_scrollBody" style="position: relative; overflow: auto; width: 100%;"><table id="defaultDataTable" class="table table-bordered table-hover nowrap dataTable no-footer" role="grid"><thead>
              <tr role="row" style="height: 0px;"><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 233.398px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">货币</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 321.016px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">别名</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 321.016px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">可用余额</div></th><th class="sorting_disabled" rowspan="1" colspan="1" style="padding-top: 0px; padding-bottom: 0px; border-top-width: 0px; border-bottom-width: 0px; height: 0px; width: 252.57px;"><div class="dataTables_sizing" style="height: 0px; overflow: hidden;">冻结中</div></th></tr></thead>
              
              <tbody><tr role="row" class="odd"><td>CNY</td><td>人民币</td><td>0</td><td>0</td></tr><tr role="row" class="even"><td>USDT</td><td>USDT</td><td>0</td><td>0</td></tr><tr role="row" class="odd"><td>INR</td><td>印度卢比</td><td>0</td><td>0</td></tr><tr role="row" class="even"><td>VND</td><td>越南盾</td><td>0</td><td>0</td></tr></tbody>
            </table></div></div><div id="defaultDataTable_processing" class="dataTables_processing panel panel-default" style="display: none;">处理中...</div></div></div><div class="row"><div class="col-sm-5"></div><div class="col-sm-7"></div></div></div>
          </div>
        </div>
  </div>
</template>

<script>
import { mapGetters } from "vuex";
// import { getList } from '@/api/table'

export default {
  name: "Balance",
  computed: {
    ...mapGetters(["name"]),
  },
  data() {
    return {
      list: {
        currency: "CNY",
        name: "asdfasdf",
        balance: "asdfasdf",
        freez: "123",
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
