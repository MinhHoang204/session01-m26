<template>
  <div>
    <h1>Thông tin cá nhân</h1>
    <p>Họ và tên: {{ user.fullName }}</p>
    <p>Giới tính: {{ user.gender }}</p>
    <p>Ngày sinh: {{ user.dob }}</p>
    <p>Email: {{ user.email }}</p>
    <p>Địa chỉ: {{ user.address }}</p>
  </div>
</template>

<script>
export default {
  name: 'UserInfo',
  data() {
    return {
      user: {
        fullName: 'Nguyễn Minh Hoàng',
        gender: 'Nam',
        dob: '11/11/2004',
        email: 'miinhhoangg204@gmail.com',
        address: 'Bắc Ninh'
      }
    }
  }
}
</script>
