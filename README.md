# bem-vindo


<div id="app"></div>
    <div class="user">
      <img id="user-photo" src="https://dkrn4sk0rn31v.cloudfront.net/uploads/2018/05/07115516/maneiras-estudar-programacao-380x350.jpg">
      <h1>Olá, <span id="user-name">visitante</span>!</h1>
      <p id="user-email"></p>
    </div>
    <div class="g-signin2" data-onsuccess="onSignIn" data-theme="dark" data-width="370" data-height="50" data-longtitle="true" data-lang="pt-BR"></div>
 
    <script>
      function onSignIn(response) {
            // Conseguindo as informações do seu usuário:
            var perfil = response.getBasicProfile();
 
            // Conseguindo o ID do Usuário
            var userID = perfil.getId();
 
            // Conseguindo o Nome do Usuário
            var userName = perfil.getName();
 
            // Conseguindo o E-mail do Usuário
            var userEmail = perfil.getEmail();
 
            // Conseguindo a URL da Foto do Perfil
            var userPicture = perfil.getImageUrl();
 
            document.getElementById('user-photo').src = userPicture;
            document.getElementById('user-name').innerText = userName;
            document.getElementById('user-email').innerText = userEmail;
 
            // Recebendo o TOKEN que você usará nas demais requisições à API:
            var LoR = response.getAuthResponse().id_token;
            console.log("~ le Tolkien: " + LoR);
        };
    </script>
  

<form>
  <div class="form-group">
    <label for="exampleInputEmail1">Endereço de email</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Seu email">
    <small id="emailHelp" class="form-text text-muted">Nunca vamos compartilhar seu email, com ninguém.</small>
  </div>
  <div class="form-group">
    <label for="exampleInputPassword1">Senha</label>
    <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Senha">
  </div>
  <div class="form-group form-check">
    <input type="checkbox" class="form-check-input" id="exampleCheck1">
    <label class="form-check-label" for="exampleCheck1">Clique em mim</label>
  </div>
  <button type="submit" class="btn btn-primary">Enviar</button>
</form>
<form>
  <div class="form-group">
    <label for="exampleFormControlInput1">Endereço de email</label>
    <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="nome@exemplo.com">
  </div>
  <div class="form-group">
    <label for="exampleFormControlSelect1">Select de exemplo</label>
    <select class="form-control" id="exampleFormControlSelect1">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
  <div class="form-group">
    <label for="exampleFormControlSelect2">Exemplo de select múltiplo</label>
    <select multiple class="form-control" id="exampleFormControlSelect2">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
  <div class="form-group">
    <label for="exampleFormControlTextarea1">Exemplo de textarea</label>
    <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
  </div>
</form>
<form>
  <div class="form-group">
    <label for="exampleFormControlFile1">Exemplo de input de arquivo</label>
    <input type="file" class="form-control-file" id="exampleFormControlFile1">
  </div>
</form>
<input class="form-control form-control-lg" type="text" placeholder=".form-control-lg">
<input class="form-control" type="text" placeholder="Input padrão">
<input class="form-control form-control-sm" type="text" placeholder=".form-control-sm">
<input class="form-control" type="text" placeholder="Input só de leitura, aqui..." readonly>
<form>
  <div class="form-group row">
    <label for="staticEmail" class="col-sm-2 col-form-label">Email</label>
    <div class="col-sm-10">
      <input type="text" readonly class="form-control-plaintext" id="staticEmail" value="email@exemplo.com">
    </div>
  </div>
  <div class="form-group row">
    <label for="inputPassword" class="col-sm-2 col-form-label">Senha</label>
    <div class="col-sm-10">
      <input type="password" class="form-control" id="inputPassword" placeholder="Senha">
    </div>
  </div>
</form>
<form class="form-inline">
  <div class="form-group mb-2">
    <label for="staticEmail2" class="sr-only">Email</label>
    <input type="text" readonly class="form-control-plaintext" id="staticEmail2" value="email@exemplo.com">
  </div>
  <div class="form-group mx-sm-3 mb-2">
    <label for="inputPassword2" class="sr-only">Senha</label>
    <input type="password" class="form-control" id="inputPassword2" placeholder="Senha">
  </div>
  <button type="submit" class="btn btn-primary mb-2">Confirmar identidade</button>
</form>
<form>
  <div class="form-group">
    <label for="formControlRange">Exemplo de input range</label>
    <input type="range" class="form-control-range" id="formControlRange">
  </div>
</form>
<div class="form-check">
  <input class="form-check-input" type="checkbox" value="" id="defaultCheck1">
  <label class="form-check-label" for="defaultCheck1">
    Checkbox padrão
  </label>
</div>
<div class="form-check">
  <input class="form-check-input" type="checkbox" value="" id="defaultCheck2" disabled>
  <label class="form-check-label" for="defaultCheck2">
    Checkbox desativado
  </label>
</div>
<form>
  <div class="form-row">
    <div class="form-group col-md-6">
      <label for="inputEmail4">Email</label>
      <input type="email" class="form-control" id="inputEmail4" placeholder="Email">
    </div>
    <div class="form-group col-md-6">
      <label for="inputPassword4">Senha</label>
      <input type="password" class="form-control" id="inputPassword4" placeholder="Senha">
    </div>
  </div>
  <div class="form-group">
    <label for="inputAddress">Endereço</label>
    <input type="text" class="form-control" id="inputAddress" placeholder="Rua dos Bobos, nº 0">
  </div>
  <div class="form-group">
    <label for="inputAddress2">Endereço 2</label>
    <input type="text" class="form-control" id="inputAddress2" placeholder="Apartamento, hotel, casa, etc.">
  </div>
  <div class="form-row">
    <div class="form-group col-md-6">
      <label for="inputCity">Cidade</label>
      <input type="text" class="form-control" id="inputCity">
    </div>
    <div class="form-group col-md-4">
      <label for="inputEstado">Estado</label>
      <select id="inputEstado" class="form-control">
        <option selected>SP</option>
          <option selected>MG</option>
            <option selected>RJ</option>
              <option selected>MT</option>
        <option>...</option>
      </select>
    </div>
    <div class="form-group col-md-2">
      <label for="inputCEP">CEP</label>
      <input type="text" class="form-control" id="inputCEP">
    </div>
  </div>
  <div class="form-group">
    <div class="form-check">
      <input class="form-check-input" type="checkbox" id="gridCheck">
      <label class="form-check-label" for="gridCheck">
        Clique em mim
      </label>
    </div>
  </div>
  <button type="submit" class="btn btn-primary">Entrar</button>
</form>
<form class="needs-validation" novalidate>
  <div class="form-row">
    <div class="col-md-4 mb-3">
      <label for="validationCustom01">Primeiro nome</label>
      <input type="text" class="form-control" id="validationCustom01" placeholder="Nome" value="Mark" required>
      <div class="valid-feedback">
        Tudo certo!
      </div>
    </div>
    <div class="col-md-4 mb-3">
      <label for="validationCustom02">Sobrenome</label>
      <input type="text" class="form-control" id="validationCustom02" placeholder="Sobrenome" value="Otto" required>
      <div class="valid-feedback">
        Tudo certo!
      </div>
    </div>
    <div class="col-md-4 mb-3">
      <label for="validationCustomUsername">Usuário</label>
      <div class="input-group">
        <div class="input-group-prepend">
          <span class="input-group-text" id="inputGroupPrepend">@</span>
        </div>
        <input type="text" class="form-control" id="validationCustomUsername" placeholder="Usuário" aria-describedby="inputGroupPrepend" required>
        <div class="invalid-feedback">
          Por favor, escolha um nome de usuário.
        </div>
      </div>
    </div>
  </div>
  <div class="form-row">
    <div class="col-md-6 mb-3">
      <label for="validationCustom03">Cidade</label>
      <input type="text" class="form-control" id="validationCustom03" placeholder="Cidade" required>
      <div class="invalid-feedback">
        Por favor, informe uma cidade válida.
      </div>
    </div>
    <div class="col-md-3 mb-3">
      <label for="validationCustom04">Estado</label>
      <input type="text" class="form-control" id="validationCustom04" placeholder="Estado" required>
      <div class="invalid-feedback">
        Por favor, informe um estado válido.
      </div>
    </div>
    <div class="col-md-3 mb-3">
      <label for="validationCustom05">CEP</label>
      <input type="text" class="form-control" id="validationCustom05" placeholder="CEP" required>
      <div class="invalid-feedback">
        Por favor, informe um CEP válido.
      </div>
    </div>
  </div>
  <div class="form-group">
    <div class="form-check">
      <input class="form-check-input" type="checkbox" value="" id="invalidCheck" required>
      <label class="form-check-label" for="invalidCheck">
        Concordo com os termos e condições
      </label>
      <div class="invalid-feedback">
        Você deve concordar, antes de continuar.
      </div>
    </div>
  </div>
  <button class="btn btn-primary" type="submit">Enviar</button>
</form>

<script>
// Exemplo de JavaScript inicial para desativar envios de formulário, se houver campos inválidos.
(function() {
  'use strict';
  window.addEventListener('load', function() {
    // Pega todos os formulários que nós queremos aplicar estilos de validação Bootstrap personalizados.
    var forms = document.getElementsByClassName('needs-validation');
    // Faz um loop neles e evita o envio
    var validation = Array.prototype.filter.call(forms, function(form) {
      form.addEventListener('submit', function(event) {
        if (form.checkValidity() === false) {
          event.preventDefault();
          event.stopPropagation();
        }
        form.classList.add('was-validated');
      }, false);
    });
  }, false);
})();
</script>
<form class="was-validated">
  <div class="mb-3">
    <label for="validationTextarea">Textarea</label>
    <textarea class="form-control is-invalid" id="validationTextarea" placeholder="Required example textarea" required></textarea>
    <div class="invalid-feedback">
      Please enter a message in the textarea.
    </div>
  </div>

  <div class="custom-control custom-checkbox mb-3">
    <input type="checkbox" class="custom-control-input" id="customControlValidation1" required>
    <label class="custom-control-label" for="customControlValidation1">Olha só, esse checkbox personalizado</label>
    <div class="invalid-feedback">Exemplo de texto para feedback inválido</div>
  </div>

  <div class="custom-control custom-radio">
    <input type="radio" class="custom-control-input" id="customControlValidation2" name="radio-stacked" required>
    <label class="custom-control-label" for="customControlValidation2">Clique neste radio personalizado</label>
  </div>
  <div class="custom-control custom-radio mb-3">
    <input type="radio" class="custom-control-input" id="customControlValidation3" name="radio-stacked" required>
    <label class="custom-control-label" for="customControlValidation3">Ou clique neste outro radio personalizado</label>
    <div class="invalid-feedback">Mais exemplo de texto para feedback inválido</div>
  </div>

  <div class="form-group">
    <select class="custom-select" required>
      <option value="">Abra este menu select</option>
      <option value="1">Um</option>
      <option value="2">Dois</option>
      <option value="3">Três</option>
    </select>
    <div class="invalid-feedback">Exemplo de feedback invalido para o select</div>
  </div>

  <div class="custom-file">
    <input type="file" class="custom-file-input" id="validatedCustomFile" required>
    <label class="custom-file-label" for="validatedCustomFile">Escolher arquivo...</label>
    <div class="invalid-feedback">Exemplo de feedback inválido para input file</div>
  </div>
</form>
<html lang="pt-BR">
  <head>
    <meta charset="UTF-8">
    <meta name="google-signin-scope" content="profile email">
    <meta name="google-signin-client_id" content="SEU_ID_DO_CLIENTE">
    <script src="https://apis.google.com/js/platform.js" async defer></script>
     
    <style type="text/css">
      @import url(http://fonts.googleapis.com/css?family=Open+Sans:400italic,600italic,600,700,400);
 
      body {
        margin: 0;
        padding: 10%;
        text-align: center;
        font-family: 'Open Sans';
        background: #F8F8F8;
      }
 
      .user {
          padding: 50px 20px;
          background: #FFFFFF;
          border-radius: 2px;
          box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
          width: 330px;
          display: block;
          margin: 0 auto;
      }
 
      #user-photo {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        display: block;
        margin: 0 auto 10px auto;
      }
 
      h1 {
        display: block;
        margin: 0 auto;
        text-align: center;
        font-weight: lighter;
      }
 
      #user-name {
        color: #0066AA;
        font-weight: bold;
      }
 
      #user-email {
        display: block;
        margin: 0 auto;
        text-align: center;
        color: #0066AA;
      }
 
      .g-signin2,
      .g-signin2 .abcRioButton {
        display: block;
        margin: 20px auto 0 auto;
        text-align: center;
      }
    </style>
  </head>   
  <body>
<script type="text/javascript" src="http://code.jquery.com/jquery-2.1.3.min.js"></script>
<script type="text/javascript" src="https://assets.moip.com.br/v2/bank-account-validator.min.js"></script>
<script type="text/javascript">
  $(document).ready(function() {
    $("#validate_bank_account").click(function() {
      Moip.BankAccount.validate({
        bankNumber         : $("#bank_number").val(),
        agencyNumber       : $("#agency_number").val(),
        agencyCheckNumber  : $("#agency_check_number").val(),
        accountNumber      : $("#account_number").val(),
        accountCheckNumber : $("#account_check_number").val(),
        valid: function() {
          alert("Conta bancária válida")
        },
        invalid: function(data) {
          var errors = "Conta bancária inválida: \n";
          for(i in data.errors){
            errors += data.errors[i].description + "-" + data.errors[i].code + ")\n";
          }
          alert(errors);
        }
      });
    });
  });
</script>
<form>
  <select id="bank_number">
    <option value="001">BANCO DO BRASIL S.A.</option>
    <option value="237">BANCO BRADESCO S.A.</option>
    <option value="341">BANCO ITAÚ S.A.</option>
    <option value="104">CAIXA ECONOMICA FEDERAL</option>
    <option value="033">BANCO SANTANDER BANESPA S.A.</option>
    <option value="399">HSBC BANK BRASIL S.A.</option>
    <option value="151">BANCO NOSSA CAIXA S.A.</option>
    <option value="745">BANCO CITIBANK S.A.</option>
    <option value="041">BANCO DO ESTADO DO RIO GRANDE DO SUL S.A.</option>
  </select>

  <input id="agency_number" placeholder="Agência" type="text"/>
  <input id="agency_check_number" placeholder="Dígito da agência" type="text" />
  <input id="account_number" placeholder="Conta corrente" type="text" />
  <input id="account_check_number" placeholder="Dígito da conta corrente" type="text" />

  <input type="button" value="Validar" id="validate_bank_account" />


<img id="user-photo" src="https://organicsnewsbrasil.com.br/wp-content/uploads/2015/10/eu-posso-te-ajudar.png">
