<template>
  <el-form ref="form" name="contact" action="" method="post" netlify :model="form" label-width="120px">
    <input type="hidden" name="form-name" value="contact" />
    <header>
      <h5>We'd love to hear from you, so please contact us. Fill out the form with any information or questions and we will contact you as soon as possible.</h5>
    </header>
    <div class="form__row">
      <el-form-item label="Name">
        <el-input v-model="name"></el-input>
      </el-form-item>
      <el-form-item label="Email">
        <el-input v-model="email"></el-input>
      </el-form-item>
    </div>
    <div class="form__row">
      <el-form-item label="Type of Inquiry">
        <el-select v-model="inquiryType" placeholder="Select">
          <el-option
            v-for="item in options"
            :key="item.value"
            :label="item.label"
            :value="item.value">
          </el-option>
        </el-select>
      </el-form-item>
    </div>
    <div v-if="inquiryType === 'trip'" class="form__row">
      <el-form-item style="min-width:413px" label="Date Range">
        <el-date-picker
          v-model="date"
          type="daterange"
          range-separator="To"
          start-placeholder="Start date"
          end-placeholder="End date">
        </el-date-picker>
      </el-form-item>
    </div>
    <el-form-item label="Message">
      <el-input
        type="textarea"
        :rows="4"
        placeholder="Please input"
        v-model="textarea">
      </el-input>
    </el-form-item>
  </el-form>
</template>

<script>
  export default {
    data() {
      return {
        name: '',
        email: '',
        textarea: '',
        options: [{
          value: 'trip',
          label: 'Trip'
        }, {
          value: 'general',
          label: 'General'
        }],
        inquiryType: '',
        date: '',
        pickerOptions2: {
          shortcuts: [{
            text: 'Last week',
            onClick(picker) {
              const end = new Date();
              const start = new Date();
              start.setTime(start.getTime() - 3600 * 1000 * 24 * 7);
              picker.$emit('pick', [start, end]);
            }
          }, {
            text: 'Last month',
            onClick(picker) {
              const end = new Date();
              const start = new Date();
              start.setTime(start.getTime() - 3600 * 1000 * 24 * 30);
              picker.$emit('pick', [start, end]);
            }
          }, {
            text: 'Last 3 months',
            onClick(picker) {
              const end = new Date();
              const start = new Date();
              start.setTime(start.getTime() - 3600 * 1000 * 24 * 90);
              picker.$emit('pick', [start, end]);
            }
          }]
        },
      }
    },
    methods: {
      onSubmit() {
        console.log('submit!');
      }
    }
  }
</script>

<style lang="scss" scoped>
  form {
    margin: 0 3rem 3rem;
    padding:2rem;
    background-color:#fff;
  }

  header {
    color:#606266;
    margin-bottom:2rem;
    line-height:1.4rem;
    padding: 0 4rem;
    font-size:.9rem;
  }

  .form {
    &__row {
      margin-bottom:1rem;
      display:flex;

      &.block {
        display:block;
      }
    }
  }
  .el-date-label {
    color:#606266;
  }
  .el-date-editor {
    width:100%;
  }
  .el-form-item {
    margin-bottom:0;
  }
  .el-range-separator {
    width: 27px !important;
  }
</style>
