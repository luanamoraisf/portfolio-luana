<template>
    <section id="about-me">
        <div class="text-[#EFEFF0] font-serif flex justify-between mt-28 mb-12">
            <h1>Formação Acadêmica</h1>
            <h1>Experiência Profissional</h1>
        </div>
        
        <div id="line-education"></div>
        <div id="line-professional"></div>

        <div id="line-horizontal1"></div>
        <div id="line-horizontal2"></div>
        <div id="line-horizontal3"></div>
        <div id="line-horizontal4"></div>

        <div class="text-[#EFEFF0] text-xsm mr-96 -mt-5">
            <h2 class="mr-56">Análise e Desenvolvimento de Sistemas</h2>
            <h2 class="mr-56">Centro Universitário Maurício de Nassau</h2>
            <h2 class="edu">2021 - 2024</h2>
        </div>
        
        <div class="text-[#EFEFF0] text-xsm mr-96 mt-32">
            <h2 class="mr-96">Informática para Internet</h2>
            <h2 class="mr-60">Instituto Federal de Pernambuco - IFPE</h2>
            <h2 class="edu">2019 - 2021</h2>
        </div>

        <div class="text-[#EFEFF0] text-xsm ml-96 -mt-96 -mr-14">
            <h2 class="ml-96 mt-10">Desenvolvedora de Software FullStack</h2>
            <h2 class="ml-36">Viitra Inovações</h2>
            <h2 class="ml-44">04/2022 - 06/2024</h2>
        </div>
        
        <div class="text-[#EFEFF0] text-xsm ml-96 -mr-14 mt-36">
            <h2 class="ml-96 -mt-2">Desenvolvedora de Software FullStack</h2>
            <h2 class="ml-64">Verdanatech Soluções em TI</h2>
            <h2 class="ml-40">07/2021 - 02/2022</h2>
        </div>
    </section>
    
</template>

<script>
export default {

}
</script>

<style>
#about-me{
    padding-top: 1%;
    margin-bottom: 25%;
}
#line-education{
    height: 600px;
    border-left: 2px solid #be61c0;
}
#line-professional{
    height: 600px;
    border-right: 2px solid #be61c0;
    margin-top: -49.4%;
    margin-right: 40%;
}
#line-horizontal1{
    width: 30px;
    border: 1px solid #be61c0;
    margin-top: -40%;
}
#line-horizontal2{
    width: 30px;
    border: 1px solid #be61c0;
    margin-top: 20%;
}
#line-horizontal3{
    width: 30px;
    border: 1px solid #be61c0;
    margin-left: 60%;
}
#line-horizontal4{
    width: 30px;
    border: 1px solid #be61c0;
    margin-left: 60%;
    margin-top: -20%;
}
.edu{
    margin-right: 64%;
}
</style>