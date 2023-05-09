<template>
    Alas : <input type="number" v-model="alas" v-on:keyup="hitung" placeholder="Alas">
    <br>
    Tinggi : <input type="number" v-model="tinggi" v-on:keyup="hitung" placeholder="Tinggi">
    <br>
    <br>
    Menghitung Luas Segitiga:
    <br>

    Alas : {{ alas }}
    <br>
    Tinggi: {{ tinggi }}
    <br>
    Luas : {{ luas }}
</template>

<script>
export default {
    data() {
        //Isiniasi variabel
        return {
            alas: null,
            tinggi: null,
            luas: null
        };
    },
    methods: {
        // function menghitung luas
        hitung() {
            this.luas = (this.alas * this.tinggi) / 2
        }
    }

}
</script>