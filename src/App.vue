<template>
  <div>
    <el-countdown format="DD [days] HH:mm:ss" :value="holiday51" style="font-size: xx-large;font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">
      <template #title>
        <div style= "align-items: center;font-size: xx-large;font-family: Hanzipen SC,serif	;">
          <el-icon style="margin-right: 4px" :size="28">
            <Calendar />
          </el-icon>
          距离五一假期还有:
        </div>
      </template>
    </el-countdown>
    <el-countdown format="DD [days] HH:mm:ss" :value="dragonBoatFestival" style="font-size: xx-large;font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">
      <template #title>
        <div style= "align-items: center;font-size: xx-large;font-family: Hanzipen SC,serif	;">
          <el-icon style="margin-right: 4px" :size="28">
            <Calendar />
          </el-icon>
          距离端午假期还有:
        </div>
      </template>
    </el-countdown>
    <el-countdown format="DD [days] HH:mm:ss" :value="moonFestival" style="font-size: xx-large;font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">
      <template #title>
        <div style= "align-items: center;font-size: xx-large;font-family: Hanzipen SC,serif	;">
          <el-icon style="margin-right: 4px" :size="28">
            <Calendar />
          </el-icon>
          距离中秋假期还有:
        </div>
      </template>
    </el-countdown>
    <el-countdown format="DD [days] HH:mm:ss" :value="holiday101" style="font-size: xx-large;font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">
      <template #title>
        <div style= "align-items: center;font-size: xx-large;font-family: Hanzipen SC,serif	;">
          <el-icon style="margin-right: 4px" :size="28">
            <Calendar />
          </el-icon>
          距离十一假期还有:
        </div>
      </template>
    </el-countdown>
    <el-countdown format="DD [days] HH:mm:ss" :value="yuanDan" style="font-size: xx-large;font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">
      <template #title>
        <div style= "align-items: center;font-size: xx-large;font-family: Hanzipen SC,serif	;">
          <el-icon style="margin-right: 4px" :size="28">
            <Calendar />
          </el-icon>
          距离元旦假期还有:
        </div>
      </template>
    </el-countdown>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import dayjs from 'dayjs'
import { Calendar } from '@element-plus/icons-vue'

const holiday51 = ref(dayjs('2024-04-30 19:30:00'))
const dragonBoatFestival = ref(dayjs('2024-06-07 19:30:00'))
const moonFestival = ref(dayjs('2024-09-14 19:30:00'))
const holiday101 = ref(dayjs('2024-09-30 19:30:00'))
const yuanDan = ref(dayjs('2024-12-31 19:30:00'))

</script>

<style scoped>
</style>
