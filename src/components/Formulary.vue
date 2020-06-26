<template>
  <div class="row formulary-page" aria-live="off">
    <div class="formulary-body">
    <h1 :style="fontSecondary">
      Peça já seu cartão
    </h1>
      <div class="col-sm-12">
        <h2 :style="fontSecondary" class="step">passo 1 de 5</h2>
        <h2 :style="fontPrimary">vamos lá</h2>
      </div>

      <div class="col-sm-12">
        <p class="descricaoH2">
          Preencha os campos abaixo com informações válidas,
          pois as usaremos como forma de contato caso sua proposta seja aprovada.
        </p>
      </div>

      <div class="col-sm-12 box">
        <label
          :style="fontPrimary"
          id="lbl_NomeCliente"
          >
          nome completo
        </label>
        <input
          :style="fontSecondary"
          aria-labelledby="lbl_NomeCliente erro-NomeCliente"
          aria-required="true"
          class="text-box single-line"
          data-val="true"
          id="NomeCliente"
          name="NomeCliente"
          placeholder="Seu nome aqui"
          type="text"
          value
          maxlength="60"
        />
        <span class="msg-erro col-12 ocultar">
          <i aria-hidden="true" class="iconeErro" />
          <span id="erro-NomeCliente" class="erro" />
        </span>
      </div>
      <div class="col-sm-6 box">
        <label
          :style="fontPrimary"
          id="lbl_Cpf"
          >
          CPF
        </label>
        <input
          aria-labelledby="lbl_Cpf erro-Cpf"
          aria-required="true"
          class="text-box single-line"
          data-val="true"
          id="Cpf"
          name="Cpf"
          placeholder="000.000.000-00"
          type="tel"
          value
          maxlength="14"
          autocomplete="off"
        />
        <span class="msg-erro col-12 ocultar">
          <i aria-hidden="true" class="iconeErro"></i>
          <span id="erro-Cpf" class="erro"></span>
        </span>
      </div>
      <div class="col-sm-6 box">
        <label
          :style="fontPrimary"
          id="lbl_Celular"
          >
          celular
        </label>
        <input
          aria-labelledby="lbl_Celular erro-Celular"
          aria-required="true"
          class="text-box single-line"
          data-val="true"
          id="Celular"
          name="Celular"
          placeholder="(00) 00000-0000"
          type="tel"
          value
          maxlength="14"
          autocomplete="off"
        />
        <span class="msg-erro col-12 ocultar">
          <i aria-hidden="true" class="iconeErro"></i>
          <span id="erro-Celular" class="erro"></span>
        </span>
      </div>
      <div class="col-sm-12 box">
        <label
          :style="fontPrimary"
          id="lbl_Email"
          >
          e-mail
        </label>
        <input
          aria-labelledby="lbl_Email erro-Email"
          aria-required="true"
          class="text-box single-line"
          data-val="true"
          id="Email"
          name="Email"
          placeholder="Coloque seu e-mail aqui"
          type="email"
          value
          maxlength="80"
        />
        <span class="msg-erro col-12 ocultar">
          <i aria-hidden="true" class="iconeErro"></i>
          <span id="erro-Email" class="erro"></span>
        </span>
      </div>
    </div>
    <div id="Box-aviso">
      <div class="col-sm-12">
        <span>
          Ao avançar, você autoriza o Emissor a consultar o Sistema de Informações de Crédito
          (SCR) do Banco Central e está ciente de que seus dados serão registrados
          do Banco Central e está ciente de que seus dados serão registrados no
          <a href="javascript:void();" data-toggle="modal" data-target="#scrModal">(SCR)</a>.
        </span>

        <span style="padding:0; padding-left:0.9375rem; min-height:70px;">
          Este site usa cookies e dados pessoais de acordo com os nossos
          <a
            href="https://www.itau.com.br/seguranca/termos-de-uso/"
            target="_blank"
          >
            Termos de Uso e Política de Privacidade
          </a>
            e, ao continuar navegando neste site, você concorda com suas condições.
        </span>
      </div>
    </div>

    <div class="modal fade" id="scrModal" tabindex="-1" role="dialog">
      <div class="modal-dialog modal-dialog-centered modal-md" role="document">
        <div class="modal-content conteudo-modal">
          <div class="modal-header">
            <h5
              class="modal-title titulo-modal"
              id="scrTitulo"
            >Sistema de Informações de Crédito (SCR)</h5>
            <button type="button" class="close" data-dismiss="modal" aria-label="Fechar">
              <span class="icon-itaufonts_fechar quero-cartao-laranja" aria-hidden="true"></span>
            </button>
          </div>
          <div class="modal-body">
            <p>
1. Você autoriza, a qualquer tempo, mesmo após o término deste contrato, o Emissor,
as sociedades do Conglomerado Itaú Unibanco e as demais instituições aptas a consultar o SCR nos
termos da regulamentação vigente e que adquiram ou recebam em garantia ou manifestem interesse de
adquirir ou receber em garantia, total ou parcialmente, operações de crédito de sua responsabilidade
("Instituições Autorizadas"), a consultar no SCR informações ao seu respeito.
            </p>
&lt; p&gt;1.1 Você declara-se ciente de que as consultas ao SCR serão realizadas com base na
presente autorização.
            <p>
1.2 Você declara, ainda, ciência de que os dados das operações de crédito que realizar serão
fornecedios ao BACEN e registrados no SCR, inclusive informações sobre o montante das suas
dívidas a vencer e vencidas, inclusive em atraso e as operações baixadas com prejuízo, bem como o
valor das coobrigações que tenha assumido e das garantias que tenha prestado, valendo essa
declaração como comunicação prévida desses registros.
            </p>
            <p>
1.3 Você poderá ter acesso, a qualquer tempo, aos seus dados no SCR pelos meios colocados à
disposição pelo BACEN, inclusive seu site e, em caso de divergência nos dados do SCR fornecidos
pelas Instituições Autorizadas, pedir sua correção, exclusão ou registros de manifestação de
discordância, bem como cadastramento de medidas judiciais, mediante a solicitação direcionada à
central de atendimento da Instituição que efetivou o registro dos dados SCR.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Formulary',
  data() {
    return {
      errors: [],
      name: null,
      age: null,
      movie: null,
      colorPrimary: '#EC7020',
      colorSecondary: '#0D456F',
    };
  },
  computed: {
    fontPrimary() {
      return {
        color: this.colorPrimary,
      };
    },
    fontSecondary() {
      return {
        color: this.colorSecondary,
      };
    },
  },
  methods: {
    checkForm(e) {
      if (this.name && this.age) {
        return true;
      }

      this.errors = [];

      if (!this.name) {
        this.errors.push('O nome é obrigatório.');
      }
      if (!this.age) {
        this.errors.push('A idade é obrigatória.');
      }

      e.preventDefault();
      return null;
    },
  },
};
</script>

<style scoped>
  .formulary-page {
    padding: 16px;
    min-width: 320px;
    width: 80%;
    margin: 0 auto;
  }
  .formulary-body {
    min-width: 320px;
    width: 70%;
    margin: 0 auto;
  }

  p, span, label {
    font-family: Arial, Helvetica, sans-serif;
  }
  h1, h2 {
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 600;
  }
  .step {
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 600;
    font-size: 12px;
  }

  input {
    font-family: Arial, Helvetica, sans-serif;
  }
</style>
