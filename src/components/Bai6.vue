<template>
  <div>
    <h1>Họ và tên: {{ fullName }}</h1>
  </div>
</template>

<script>
export default {
  name: 'FormatName',
  data() {
    return {
      user: {
        firstName: 'Nguyễn Văn',
        lastName: 'Nam'
      },
      fullName: ''
    }
  },
  methods: {
    formatName(user) {
      return `${user.firstName} ${user.lastName}`;
    }
  },
  mounted() {
    this.fullName = this.formatName(this.user);
  }
}
</script>