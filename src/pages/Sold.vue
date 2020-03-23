<template>
  <q-page class="">
    <div class="container">
        <h2 class="text-center">Stock Product</h2>
        <div class="table">
        <q-table
            title="Stock & Sold Product"
            class="bg-grey-3"
            :data="data"
            :columns="columns"
            row-key="name"
    />
        </div>
        <!-- <Test></Test> -->
    </div>
  </q-page>
</template>

<script>
// import Test from 'components/Test'

export default {
  name: 'Sold',

  // components: {
  //   Test
  // },

  data () {
    return {
      columns: [
        {
          name: 'name',
          required: true,
          label: 'name product',
          align: 'left',
          field: row => row.name,
          format: val => `${val}`,
          sortable: true
        },
        { name: 'categories', align: 'center', label: 'categories', field: 'categories', sortable: true },
        { name: 'month', label: 'Month', field: 'Month', sortable: true },
        { name: 'month', label: 'Year', field: 'Year', sortable: true },
        { name: 'sold', label: 'Sold', field: 'Sold' },
        { name: 'stock', label: 'Stock (g)', field: 'Stock' }
      ],
      data: [
        {
          name: 'Classic sound',
          categories: 'Piano',
          Month: 'january',
          Year: '2020',
          Sold: '20',
          Stock: '30'
        },
        {
          name: 'Gibson black',
          categories: 'Guitar',
          Month: 'january',
          Year: '2020',
          Sold: '22',
          Stock: '50'
        },
        {
          name: 'Dw guardian',
          categories: 'Drum',
          Month: 'january',
          Year: '2020',
          Sold: '11',
          Stock: '22'
        },
        {
          name: 'Biola sandwood',
          categories: 'Biola',
          Month: 'january',
          Year: '2020',
          Sold: '6',
          Stock: '12'
        }]
    }
  }
}
</script>

<style>
    .table {
        width: 90%;
        border: 1px solid lightgray;
        margin: auto;
    }
    .q-page {
      padding-top: 40px;
      background-color: lightgray;
    }
</style>
