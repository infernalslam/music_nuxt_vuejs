<template>
<div>

<el-form label-position="top">


  <h3 class="main-title"> List Working </h3>
  <el-form-item label="Working Type:">
    <el-select v-model="value" placeholder="Select" size="small">
      <el-option 
        v-for="item in options"
        :key="item.label"
        :label="item.label"
        :value="item.value">
      </el-option>
    </el-select>
  </el-form-item>

  <h3 class="main-title"> Detals Working: </h3>


  </el-form>

</div>
</template>

<script>
export default {
  layout: 'menu',
  data () {
    return {
      value: '',
      options: [{label: 'เร่งด่วน', value: '1'}, {label: 'ธรรมดา', value: '2'}]
    }
  }
}
</script>
