<template>
    <div>
        <h2>User {{ id }}</h2>
        <!-- <router-link :to="id + '/profile'">profile</router-link> -->
        <router-link :to="{ name : 'profile' }">profile</router-link>
    
        <router-view></router-view>
    </div>
</template>

<script>
export default {
    props: ['id']
}
</script>
