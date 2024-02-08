<template>
      <el-countdown format="DD [days] HH:mm:ss" :value="qm" style="font-size: xx-large;font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">
        <template #title>
          <div style= "align-items: center;font-size: xx-large;font-family: Hanzipen SC	;">
            <el-icon style="margin-right: 4px" :size="28">
              <Calendar />
            </el-icon>
            距离清明节还有:
          </div>
        </template>
      </el-countdown>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
import dayjs from 'dayjs'
import { Calendar } from '@element-plus/icons-vue'

const value2 = ref(dayjs().add(1, 'month').startOf('month'))
const qm = ref(dayjs('2024-04-04'))
const djs = dayjs()
const value3 = ref(qm.value)

</script>

<style scoped>
</style>
