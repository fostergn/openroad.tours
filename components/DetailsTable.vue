<template>
  <div class="table__container">
    <el-table
      :summary-method="total"
      show-summary
      sum-text="Price per person"
      :data="tableData"
      style="width: auto">
      <el-table-column
        prop="included"
        label="Included">
      </el-table-column>
      <el-table-column
        prop="notIncluded"
        label="Not Included">
      </el-table-column>
    </el-table>
  </div>
</template>

<script>
  export default {
    methods: {
      total ({ columns, data }) {

        return ['Price Per Person', '$1350 USD'];
      }
    },
    data() {
      return {
        tableData: [
          {
            included: '2017 Honda CRF 250cc',
            notIncluded: 'Flights'
          },
          {
            included: 'Gas',
            notIncluded: 'Insurance'
          },
          {
            included: 'On-Route Maintentance',
            notIncluded: 'Drinks'
          },
          {
            included: 'Accomdation for 8 Days',
            notIncluded: 'Non-Itinerary Items'
          },
          {
            included: 'Food (breakfast, lunch, and dinner)',
            notIncluded: ''
          },
          {
            included: 'Visas',
            notIncluded: ''
          }
        ]
      }
    }
  }
</script>

<style lang="scss">
  .table__container {
    width:50%;
  }

  .el-table {
    margin:1rem;
    box-shadow: 0 1px 3px rgba(0,0,0,0.12), 0 1px 2px rgba(0,0,0,0.24);
  }

  th, td {
    color:#999;
  }

  th:first-child {
    font-weight:600;
  }

  th:first-child, td:first-child {
    color: #333;
  }
</style>
