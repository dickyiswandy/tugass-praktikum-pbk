<template>
    <v-app-bar app color="black" dark flat class="px-12">
        <v-btn>
            <v-icon color="yellow" left class="mr-2">fas fa-signature</v-icon>Dicky Iswandy
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('home')" class="text-yellow">home</v-btn>
        <v-btn text @click="scroll('about')" >about</v-btn>
        <v-btn text @click="scroll('portfolio')" >Portfolio</v-btn>
        <v-btn text @click="scroll('service')" >service</v-btn>
        <v-btn text @click="scroll('page')" >Page</v-btn>
        <v-btn text @click="scroll('biodata')" >Biodata</v-btn>
        <v-btn text @click="scroll('contact')" >Contact</v-btn>
    </v-app-bar>
</template>

<script>
export default{
    methods: {
        scroll(refName) {
            const element = document.getElementById(refName);
            element.scrollIntoView({behavior: "smooth"});
        }
    }
}
</script>

<style>

</style>