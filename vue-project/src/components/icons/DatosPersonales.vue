<script setup>
const title = 'Karen Céspedes Rivas';
const descripcion = 'Técnico Universitario en Programación';
const residencia = 'San Rafael, Mendoza, Argentina';
const presentacion = 'Hola, bievenido a mi portfolio de proyectos. Soy un desarrollador web con experiencia en el desarrollo de aplicaciones web.'
const redesSociales = [
    {id: 1, name:'Linkedin', src:'/src/assets/linkedin_icon.svg' , url:'https://www.linkedin.com/in/karen-cespedes-rivas-kcr180694/'},
    {id: 2, name:'gmail', src:'/src/assets/linkedin_icon.svg' , url:'cesp.karen@gmail.com'},
    {id: 3, name:'Github', src:'/src/assets/linkedin_icon.svg' , url:'https://github.com/karenCespedesR'},
    {id: 4, name:'Curriculum', src: '/src/assets/linkedin_icon.svg', url:'https://drive.google.com/file/d/1BsEPBECel0b4O230gCC0bFlXG0XtiEin/view?usp=sharing'}

];

const telefono = +5491130683971
</script>

<template>

<section class="datos-personales">
    <div class="card">
        <h1>{{ title }}</h1>
        <h2>{{ descripcion }}</h2>
        <p>{{ presentacion }}</p>
        <ul class="container-lista">
            <li v-for = "red in redesSociales" :key="red.id">
                <a :href="red.url"><img class="icon-redsocial" :src="red.src" width="35rem" :alt="red.name"></a>
            </li>
        </ul>
        <h3>Mi Telefono personal: {{ telefono }}</h3>
        <h4>{{ residencia }}</h4>
    </div>
</section>
</template>
<style scoped>
h1{
    font-size: 2.5rem;
}
p{
    font-size: 1.2rem;
    font-weight: 600;
    margin-bottom: 1rem;
}
.card{
    background-color: rgb(28,41,52);
    border-radius: 10px;
    padding: 10px;
    margin: 10px;
    text-align: center;
}
.container-lista{
    display: flex;
    justify-content: center;
    list-style: none;
    padding: 0;
    margin: 0;
    text-align: center;
}

.icon-redsocial{
    align-items: center;
    background-color: aliceblue;
    border-radius: 50%;

}
.icon-redsocial:hover{
    background-color: rgb(28,41,52);
    box-shadow: 0 0 5px rgba(251,249,249,0.934);
}
h3{
    font-size:1.2rem;
    font-weight: 600;
}
</style>

