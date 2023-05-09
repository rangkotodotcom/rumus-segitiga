<template>
    Email : <input type="text" v-bind:value="email" placeholder="Email">
    <br>
    Nama : <input type="text" v-model="nama" placeholder="Nama">
    <br>
    <br>

    Email : {{ email }}
    <br>
    Nama: {{ nama }}
</template>

<script>
export default {
    data() {
        //Isiniasi variabel
        return {
            email: "email@domain.com",
            nama: null
        };
    },
}
</script>