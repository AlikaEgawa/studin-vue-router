<template>
    <nav>
        <h2>Users</h2>
        <router-link
            to="/"
            active-class="link--active"
            exact
            class="link"
            style="padding-right: 15px;"
        >Home</router-link>
        <router-link
            to="/users"
            active-class="link--active"
            exact
            class="link"
        >Users</router-link>
    </nav>
</template>