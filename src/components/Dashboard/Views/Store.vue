<template>
    <div class="row">
      <div class="col-md-12">
        <div class="card">
          <paper-table :title="table1.title" :sub-title="table1.subTitle" :data="table1.data" :columns="table1.columns">

          </paper-table>
        </div>
      </div>

    </div>
</template>
<script>
  import PaperTable from 'components/UIComponents/PaperTable.vue'
  const tableColumns = ['Id', 'Name', 'Price', 'CreatedAt', 'UpdatedAt', 'SellerName']
  const tableData = [{
    id: 1,
    name: 'car',
    price: '$36.738',
    createdat: '3/2/2018',
    updatedat: '4/2/2018',
    sellername: 'Liza Charles'
  },
  {
    id: 2,
    name: 'puppy',
    price: '$99.738',
    createdat: '2/2/2018',
    updatedat: '3/2/2018',
    sellername: 'Youssef Rami'
  },
  {
    id: 3,
    name: 'hat',
    price: '$99.738',
    createdat: '1/2/2018',
    updatedat: '6/2/2018',
    sellername: 'Farah Wael'
  },
  {
    id: 4,
    name: 'plane',
    price: '$999999.738',
    createdat: '8/2/2018',
    updatedat: '12/2/2018',
    sellername: 'Omar Zakaria'
  },
  {
    id: 5,
    name: 'glasses',
    price: '$899.738',
    createdat: '8/2/2018',
    updatedat: '16/2/2018',
    sellername: 'Samira Mahomoud'
}
]

  export default {
    components: {
      PaperTable
    },
    data () {
      return {
        table1: {
          title: 'COMPONENT4 ',
          subTitle: 'GUC BAZAR',
          columns: [...tableColumns],
          data: [...tableData]
        },
        table2: {
          title: 'Table on Plain Background',
          subTitle: 'Here is a subtitle for this table',
          columns: [...tableColumns],
          data: [...tableData]
        }
      }
    }
  }

</script>
<style>

</style>
