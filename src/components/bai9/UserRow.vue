<template>
  <tr>
    <td>{{ user.id }}</td>
    <td>{{ user.name }}</td>
    <td>{{ user.dob }}</td>
    <td>{{ user.gender }}</td>
    <td>{{ user.address }}</td>
    <td>
      <button class="edit-btn">Sửa</button>
      <button class="delete-btn">Xóa</button>
    </td>
  </tr>
</template>

<script>
export default {
  name: 'UserRow',
  props: {
    user: Object,
  },
};
</script>

<style scoped>
.edit-btn, .delete-btn {
  background-color: red;
  color: white;
  border: none;
  padding: 5px 10px;
  margin: 0 5px;
  cursor: pointer;
}

.edit-btn:hover, .delete-btn:hover {
  background-color: darkred;
}
</style>
