<template>
    a : {{ alas }}
    <br>
    t: {{ tinggi }}
    <br>
    maka luas segitiganya : {{ luas }}
</template>

<script>
export default {
    data() {
        //Isiniasi variabel
        return {
            alas: 20,
            tinggi: 10
        };
    },
    computed: {
        luas() {
            return (this.alas * this.tinggi) / 2
        }
    }

}
</script>