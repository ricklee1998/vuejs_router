<template>
    <div>
        <h3>User: {{ id }} Profile</h3>
    </div>
</template>

<script>
export default {
    props: ['id']
}
</script>
<style>
h3 {
  color: #ff0037;
}
</style>