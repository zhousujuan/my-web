<template>
  <el-menu
    active-text-color="#ffd04b"
    background-color="#172032"
    class="el-menu-vertical-demo"
    default-active="2"
    text-color="#fff"
    @open="handleOpen"
    @close="handleClose"
  >
    <el-sub-menu index="1">
      <template #title>
        <el-icon><location /></el-icon>
        <span>应用</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="1-1">应用列表</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>
    <el-sub-menu index="2">
      <template #title>
        <el-icon><location /></el-icon>
        <span>发布</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="2-1">发布管理</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>

    <el-sub-menu index="3">
      <template #title>
        <el-icon><location /></el-icon>
        <span>可观测性</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="3-1">应用概览</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>

    <el-sub-menu index="4">
      <template #title>
        <el-icon><location /></el-icon>
        <span>监控告警</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="4-1">监控查询</el-menu-item>
        <el-menu-item index="4-2">监控统计</el-menu-item>
        <el-menu-item index="4-3">监控描述</el-menu-item>
        <el-menu-item index="4-4">告警记录</el-menu-item>
        <el-menu-item index="4-5">告警配置</el-menu-item>
        <el-menu-item index="4-6">告警角色</el-menu-item>
        <el-menu-item index="4-7">系统监控</el-menu-item>
        <el-menu-item index="4-8">应用监控</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>

    <el-sub-menu index="5">
      <template #title>
        <el-icon><location /></el-icon>
        <span>日志账单</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="5-1">日志查询</el-menu-item>
        <el-menu-item index="5-2">账单查询</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>

    <el-sub-menu index="6">
      <template #title>
        <el-icon><location /></el-icon>
        <span>资源管理</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="6-1">资源池</el-menu-item>
        <el-menu-item index="6-2">资源使用情况</el-menu-item>
        <el-menu-item index="6-3">资源申请审批</el-menu-item>
        <el-menu-item index="6-4">持久卷管理</el-menu-item>
        <el-menu-item index="6-5">K8S集群管理</el-menu-item>
        <el-menu-item index="6-6">资源池管理</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>
    <el-sub-menu index="7">
      <template #title>
        <el-icon><location /></el-icon>
        <span>数据资源</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="7-1">数据源</el-menu-item>
        <el-menu-item index="7-2">路由管理</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>

    <el-sub-menu index="8">
      <template #title>
        <el-icon><location /></el-icon>
        <span>运营工具</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="8-1">运营工具</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>

    <el-sub-menu index="9">
      <template #title>
        <el-icon><location /></el-icon>
        <span>权限管理</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="9-1">权限管理</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>

    <el-sub-menu index="10">
      <template #title>
        <el-icon><location /></el-icon>
        <span>帮助</span>
      </template>
      <el-menu-item-group>
        <el-menu-item index="10-1">开发文档</el-menu-item>
      </el-menu-item-group>
    </el-sub-menu>
  </el-menu>
</template>

<script lang="ts" setup>
import { ref } from "vue";
import {
  Location,
  Document,
  Menu as IconMenu,
  Setting,
} from "@element-plus/icons-vue";

const isCollapse = ref(false);
const handleOpen = (key: string, keyPath: string[]) => {
  console.log(key, keyPath);
};
const handleClose = (key: string, keyPath: string[]) => {
  console.log(key, keyPath);
};
</script>
