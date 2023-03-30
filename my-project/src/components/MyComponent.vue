<template>
  <div>
    <h1>{{ message }}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "Child Component",
    };
  },
  mounted() {
    console.log("This component is mounted");
  },
  beforeUnmount() {
   console.log("Before Unmount");
   //Dùng để thực hiện các tác vụ như hủy các kết nối, xóa các listeners, hoặc lưu trữ trạng thái của component.
  },
  unmounted() {
   console.log(" Unmounted");
   //Dùng để thực hiện các tác vụ như giải phóng bộ nhớ, hoặc gửi log để theo dõi hoạt động của component.
  },
};
</script>
