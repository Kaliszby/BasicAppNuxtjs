<template>
  <!-- _name คือการสร้างชื่อตัวแปรรับพารามิเตอร์ -->
  <h2>Welcome :{{ $route.params.name }}</h2>
</template>

<script>
export default {
  // validate params โดยใช้ regex ให้รับค่าแค่ตัวเลข
  validate(data) {
    return /^\d+$/.test(data.params.name)
  },
}
</script>
