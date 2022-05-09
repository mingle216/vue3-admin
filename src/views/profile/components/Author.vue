<template>
  <div class="author-container">
    <div class="header">
      <my-avatar
        image="https://wx-login.oss-cn-shanghai.aliyuncs.com/upload/%E5%A4%B4%E5%83%8F/avatar3.jpg"
        height="60px"
        width="60px"
        :hoverable="false"
      >
        {{ $t('msg.profile.name') }}
      </my-avatar>
      <div class="header-desc">
        <h3>{{ $t('msg.profile.name') }}</h3>
        <span>{{ $t('msg.profile.job') }}</span>
      </div>
    </div>
    <div class="info">
      {{ $t('msg.profile.Introduction') }}
    </div>
  </div>
</template>

<script setup>
import MyAvatar from '@/components/MyAvatar/index.vue'
import {} from 'vue'
</script>

<style lang="scss" scoped>
.author-container {
  .header {
    display: flex;
    .header-desc {
      margin-left: 12px;
      display: flex;
      flex-direction: column;
      justify-content: space-around;

      span {
        font-size: 14px;
      }
    }
  }
  .info {
    margin-top: 16px;
    line-height: 22px;
    font-size: 14px;
    text-indent: 26px;
  }
}
</style>
