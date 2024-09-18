<template>
  <table class="user-table">
    <thead>
      <tr>
        <th>STT</th>
        <th>Họ và tên</th>
        <th>Ngày sinh</th>
        <th>Giới tính</th>
        <th>Địa chỉ</th>
        <th>Hành động</th>
      </tr>
    </thead>
    <tbody>
      <UserRow v-for="user in users" :key="user.id" :user="user" />
    </tbody>
  </table>
</template>

<script>
import UserRow from './UserRow.vue';

export default {
  name: 'UserTable',
  components: {
    UserRow,
  },
  props: {
    users: Array,
  },
};
</script>

<style scoped>
.user-table {
  width: 100%;
  border-collapse: collapse;
}

.user-table th, .user-table td {
  border: 1px solid #ddd;
  padding: 8px;
}

.user-table th {
  background-color: #f2f2f2;
}
</style>
