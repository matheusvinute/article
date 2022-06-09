# O que é Javascript

[![Javascript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#)

Javascript foi criado por Brendan Eich e lançado em 1995 no Netscape 2.0 com o nome de Livescript, com o objetivo de validar formularios e dar dinâmica nas funcionalidades dos sites.

Esse linguagem de programação é um das mais utilizadas no mundo, tendo ganhado vários adeptos e melhorias ao longo do tempo. Seu uso hoje serve para aplicações web, mobile, IoT entre outros. Um dos grandes responsaveis por essa evolução e melhoria da liguagem se deve ao ECMA(European Computer Manifacture's Association) um organização global responsável por criar especificações de padrões para utilização da comunicação usando tecnologia, a especificação responsavel pelo Javascript é a 262.

Javascript hoje é uma liguagem multi paradigma com recursos para orientação a objetos, mas de tipagem fraca. Ela é também uma liguagme dinâmica, não sendo necessário definir os tipos das variáveis antes da compilação.

A espeficação ECMA do Javascript atual é o ES6. Possuindo as melhorias como:

## `Desestrutucação`

Ela é uma propriedade que torna possivel desestruturar valores de arrays ou propriedades de objetos em variáveis distintas, no caso dos objetos possui o rest operator(...rest), que armazenas todas as demais propriedade em um unico lugar.


  const supermercado = ['arroz', 'feijão', 'carne'];
   const [arroz, feijão] = supermercado;
   
   console.log(arroz)


 const aluno = {
      nome: "Matheus",
      idade: 20,
      escola: "Escola Municipal",
      serie: "1 ano",
      turma: "A",
      turno: "Manha"
   };
   
   const [nome, escola, turma, ...outros] = aluno;
   
   console.log(nome); //Matheus
   console.log(escola); //Escola Municipal
   console.log(turma); // A


## `Módulos`

Permitem criar codigos como funções, classes ou até mesmo variáveis que possam ser importados em outros arquivos, o que permite dividir ainda mais as funcionalidades nos codigos.


  //arquivoextra.js
  const testeModulo = () => Este é um exemplo de funcionamento de Modulos";
  
  export texteModulo;
  
  //arquivoprincipal.js
  import {texteModulo} from './arquivoextra.js';
  
  console.log(texteModulo());


## `Promisse`

E a capacidade de executar scripts em uma thread em background da thread principal. Em outras palavras, é executar mais de uma thread, sob a thread principal, sem prejudicar seu desempenho.

  function somaNumero(){
    const resultado = 1 + 1;

    if(resultado == 2){
      sucesso()
    }else{
      erro()
    }
  }

  function sucesso(){
    console.log("O resultado foi igual a 2")
  }

  function erro(){
    console.log("O resultado foi diferente de 2")
  }

  somaNumero();
