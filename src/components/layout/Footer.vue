<template>
<footer class="footer">
            <div class="col-md-5">
            <form @submit="enviar" class="gform" method="POST" data-email="yago.ayala@outlook.com"
                action="https://script.google.com/macros/s/AKfycbyCanF4Q7fXcRxKqUum3CeC12nzhQbho9BllJFXx4bQb6rzmoO3KMa_inAXOsTQi-g8fQ/exec">
                    <fieldset class="form-group">
                        <input type="form-control" name="name" id="name" class="form-control" placeholder="Nome">
                    </fieldset>
                    <fieldset class="form-group">
                        <input type="email" name="email" class="form-control" id="exampleInputEmail1" placeholder="Coloque seu E-mail">
                    </fieldset>
                    <fieldset class="form-group">
                        <textarea class="form-control" id="message" name="message" placeholder="Mensagem"></textarea>
                    </fieldset>
                    <fieldset class="form-group text-xs-right">
                        <button type="submit" class="btn btn-secondary-outline btn-lg">Enviar</button>
                    </fieldset>
                </form>
            </div>
</footer>

</template>

<script>
export default {
    methods: {
        enviar() {
            window.location.reload()
        }
    }
}
</script>

<style scoped>
.footer {
  width: 750px;
  height: 327.5px;
  margin: auto;
  background-color: #333;
}

footer {
  color: #fff;
}

footer a {
  color: #fff;
  text-decoration:none;
}

footer .form-control {
    margin-top: 15px;
    box-shadow: 0 1px 0 0 rgba(255, 255, 255, 0.1);
    border: none;
    resize: none;
    color: #fff;
    padding: 1em 1em;
    background-color: #363b48;
    width: 596px;
}

 </style>
