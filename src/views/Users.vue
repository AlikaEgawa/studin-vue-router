<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <div>
        <h3>Users</h3>
        <router-link to="/users/1">ユーザー１</router-link>
        <router-link to="/users/2">ユーザー２</router-link>
        <hr>
        <h1>User No. {{ id }}</h1>
        <router-link :to=" '/users/' + (Number(id) + 1 ) + '/profile' ">次のユーザー</router-link>
        <router-view></router-view>
    </div>
</template>

<script>
export default {
    props: ["id"],
};
</script>