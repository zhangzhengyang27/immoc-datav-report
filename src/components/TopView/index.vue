<template>
  <div class="top-view">
    <!-- :gutter="20" 指的是中间的间距   -->
    <el-row :gutter="20">
      <el-col :span="6">
        <el-card shadow="hover">
          <total-sales/>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <total-orders/>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <today-users/>
        </el-card>
      </el-col>
      <el-col :span="6">
        <el-card shadow="hover">
          <total-users/>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
import TotalSales from '../base/TotalSales'
import TotalOrders from '../base/TotalOrders'
import TodayUsers from '../base/TodayUsers'
import TotalUsers from '../base/TotalUsers'

export default {
  components: {
    TotalSales,
    TotalOrders,
    TodayUsers,
    TotalUsers
  }
}
</script>

<style lang="scss" scoped>
</style>
