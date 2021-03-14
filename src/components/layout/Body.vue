<template>
    <body class="body">

    <nav class="nav_abas">
        <ul>
            <li>
                <input type="radio" name="abas" class="abas" id="aba1">
                <label for="aba1">Introdução</label>
                <div class="conteudo">
                    <article>
                        Olá professora Tassiana Kautzmann, me chamo Yago Cristiano Costa Ayala e tenho 18 anos, sou um pouco tímido, mas 
                        ao mesmo tempo amo fazer novas amizades. Atualmente trabalho na empresa DevHero como programador junior.
                    </article>
                    <img style="margin-left:auto; float: right;" src="https://gartic.com.br/imgs/mural/fu/fullmoon/timido.png" width="375">
                </div>
            </li>
            <li>
                <input type="radio" name="abas" class="abas" id="aba2">
                <label for="aba2">Skills</label>
                <div class="conteudo">
                    <article>
                        Atualmente consigo falar 3 idiomas (português, inglês e espanhol), em relação a programação eu me considero menos pior em JS, CSS 
                        e HTML, encontro-me aprimorando nas linguagens já citadas e em Vue.js, Docker, AWS, DynamoDB, etc.
                    </article>
                    <img style="display: block; margin-left: auto; margin-right: auto;" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTD9BwaN-pzQEjc2e-AOPz0YUOssMierVD8IA&usqp=CAU" width="350">
                </div>
            </li>
            <li>
                <input type="radio" name="abas" class="abas" id="aba3">
                <label for="aba3">Defeitos</label>
                <div class="conteudo">
                    <article>
                        Hoje em dia tenho vários defeitos e julgo que eles são normais, porque eu sou um humano. Meus maiores defeitos são: a pressa, quero
                         tudo o mais rápido possível e isso me atrapalha em várias atividades; teimosia; preguiça, eu, literalmente, procrastino tudo; etc...
                    </article>
                    <img style="display: block; margin-left: auto; margin-right: auto;" src="https://i.ytimg.com/vi/v8dQl7ntM8A/maxresdefault.jpg" width="300">
                </div>
            </li>
            <li>
                <input type="radio" name="abas" class="abas" id="aba4">
                <label for="aba4">Expectativa</label>
                <div class="conteudo">
                    <article>
                        Eu espero que no futuro eu consiga evoluir muito como pessoa e como profissional, ainda estou em dúvida se irei morar no Brasil ou no exterior. 
                        Gostaria muito de fazer algo que impactasse no mundo (positivamente), é um sonho meio bobo, mas me esforço diariamente para algum dia talvez conseguir.
                    </article>
                    <img style="display: block; margin-left: auto; margin-right: auto;" src="https://content.fortune.com/wp-content/uploads/2021/02/GettyImages-1229901940.jpg" width="290">
                </div>
            </li>
                        <li>
                <input type="radio" name="abas" class="abas" id="aba5">
                <label for="aba5">Contato</label>
                <div class="conteudo">
                    <Footer />
                </div>
            </li>
        </ul>
    </nav>
    </body>

</template>

<script>
import Footer from './Footer'
export default {
    name:"Body",
    components: {
        Footer
    },
}
</script>

<style scoped>
        * {
            margin: 0;
            padding: 0;
        }

        body {
            background-color: #ddd;
            font-family: 'Roboto';
            text-align: justify;
            text-justify: inter-word;
        }

        .nav_abas {
            width: 750px;
            height: 400px;
            margin: auto;
            background-color: #fff;
            position: relative;
        }

        .nav_abas ul {
            list-style: none;
        }

        .nav_abas ul li {
            float: left;
        }

        .nav_abas label {
            width: 150px;
            padding: 25px;
            background-color: #363b48;
            display: block;
            color: #fff;
            cursor: pointer;
            text-align: center;
            font-weight: 900;
            text-transform: uppercase;
        }

        .abas:checked~label {
            background-color: #e54e43
        }

        .abas {
            display: none;
        }

        .conteudo {
            background-color: #fff;
            display: none;
            justify-content: center;
            align-items: center;
            position: absolute;
            height: 320px;
            width: 750px;
            left: 0;
        }

        .conteudo article {
            padding: 10px;
        }

        .abas:checked~.conteudo {
            display: block;
        }
</style>