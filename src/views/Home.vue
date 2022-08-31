<!-- eslint-disable vue/multi-word-component-names -->
<template>
    <div>
        <h3>Home</h3>
        <button @click="toUsers">Usersのページにいく</button>
        <p>DoubleCount : {{ doubleCount }}</p>
        <p>TripleCount : {{ tripleCount }}</p>
    </div>
</template>

<script>
import { mapGetters } from 'vuex';

export default {
    computed: {
        ...mapGetters(["doubleCount", "tripleCount"])
    },
    methods: {
        toUsers() {
            this.$router.push({
                    name: "users-id-profile",
                    params: { id: 1 }
                });
        }
    },
}
</script>