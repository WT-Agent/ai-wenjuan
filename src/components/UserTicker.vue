<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****3311 设计了新餐饮品牌价格接受度调研问卷"
  },
  {
    "text": "用户 189****6622 获得了 SaaS 软件 NPS 净推荐值量表题目"
  },
  {
    "text": "用户 131****9900 完成了 500 人企业员工满意度匿名问卷"
  },
  {
    "text": "用户 156****4455 生成了学术论文用户短视频使用时长问卷"
  },
  {
    "text": "用户 173****8811 取得了防糊弄作废数据筛选过滤 SOP"
  }
]);
</script>
