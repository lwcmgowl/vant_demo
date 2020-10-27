<template>
  <div>
    <van-sidebar v-model="activeKey">
      <van-sidebar-item title="推荐分类" ></van-sidebar-item>
      <van-sidebar-item title="超市" ></van-sidebar-item>
      <van-sidebar-item title="男装" ></van-sidebar-item>
    </van-sidebar>
  </div>
</template>
<script>
import { Sidebar, SidebarItem } from 'vant'

export default {
  data () {
    return {
      activeKey: 0
    }
  },
  components: {
    [Sidebar.name]: Sidebar,
    [SidebarItem.name]: SidebarItem
  }
}
</script>
