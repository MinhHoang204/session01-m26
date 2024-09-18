<template>
  <div>
    <h2>Danh sách khóa học</h2>
    <ol>
      <li>HTML</li>
      <li>CSS</li>
      <li>JavaScript</li>
      <li>ReactJS</li>
    </ol>
  </div>
</template>

<script>
export default {
  name: 'ListCourse',
};
</script>

<style scoped>
h2 {
  font-weight: bold;
}
ol {
  list-style-type: decimal;
}
li {
  margin: 5px 0;
}
</style>
