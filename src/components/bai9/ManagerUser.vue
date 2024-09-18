<template>
  <div class="manager-user">
    <UserTable :users="users" />
  </div>
</template>

<script>
import UserTable from './UserTable.vue';

export default {
  name: 'ManagerUser',
  components: {
    UserTable,
  },
  data() {
    return {
      users: [
        { id: 1, name: 'Medelinn Cooper', dob: '21/06/1987', gender: 'Nam', address: 'New York' },
        { id: 2, name: 'Maria', dob: '11/02/1992', gender: 'Nữ', address: 'London' },
      ],
    };
  },
};
</script>

<style scoped>
.manager-user {
  padding: 20px;
}
</style>
