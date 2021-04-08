# ROADMAP BACK-END
 
 Este roadmap de back-end contém texto que escrevi a fim de explicar o que compreendi a respeito do tópico estudado. Desta forma, talvez haja erros, tantos conceituais quanto de linguaguem, afinal errar é normal para quem está aprendendo. Caso encontre algum erro, pode me informar através de issues.

## Sumário
<details>
<summary>Mostrar conteúdo</summary>

* [Como a internet funciona?]()
* [O que é HTTP?]()
 
</details>

## Como a internet funciona?

Primeiramente é necessário compreender o que é a internet em si. Simplificamente (mas muito simplificadamente), pode-se entender a internet como uma rede que interliga diversos computadores.

Uma rede é o que permite a conexão/comunicação entre os computadores. Para que esta comunicação ocorra são necessários outros componentes que serão descritos abaixo. O site do [MDN Web docs](https://developer.mozilla.org/pt-BR/docs/Learn/Common_questions/How_does_the_Internet_work) traz um texto bem legal de conceito de redes.

Um dos integrantes de uma rede de internet é o **roteador**, que é um computador que se conecta com outros computadores, atuando como intermediador e ponto central. Este por sua vez conecta ao **modem** que permite a conexão com a rede telefonica, chamada de **ISP** _(Internt Service Provider)_. 

Para que a mensagem chegue até o destinatário, são utilizados os **IP** _(Internet Protocol)_ que é um endereço composto por 16 números. Toda página na internet tem um IP único. Para descobrir o IP de uma página é só usar o comando 

```sh
ping www.site.com
``` 

no terminal. 

### Palavrinhas interessantes
- DNS: é um banco de dados distribuido que contem o endereço IP de diversos computadores.
- TCP/IP: é um protocolo de transferência que adequa a mensagem para que seja transmitida pela rede.

## O que é HTTP?

É Hypertext Transfer Protocol, ou seja, um protocolo de transferencia de hipertexto usado pelo navegadores e servidores para se comunicarem na internet. 

Também conhecido como protocolo cliente-servidor. É usado tanto para **requisições** quanto para **respostas**.

A caracteristica do HTTP é que ele é extensível e sem estado.

O fato de ser extensível significa que pode ser adaptável, pois a variedade de itens que podem compor os cabeçalhos das mensagem.
O sem estado significa que assim que a resposta é enviada a conexão é fechada.

O que é possível controlar pelo HTTP:
- Cache;
- Restrições de origem;
- Autenticação;
- Proxy;
- Sessões.

### Vale lembrar

A porta padrão dos servidores é a 80, sendo geralmente ocultada.

### Referência bibliográfica 

* [HTTP visão geral](https://developerS.mozilla.org/pt-BR/docs/Web/HTTP/Overview)