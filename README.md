### * Atalhos WebMedia 2020
- [voc� est� aqui] Rechat: C�digo-Fonte do Painel Web
- [V�deo Demonstrativo](https://breakdance.github.io/breakdance/)
- [Artigo em PDF (ACM/Webmedia)](https://breakdance.github.io/breakdance/)
- Configura��es Tempor�rias
    - [Link do Painel Web configurado](ec2-18-228-83-110.sa-east-1.compute.amazonaws.com)
    - [Rechat: APK do Aplicativo Simulador](https://breakdance.github.io/breakdance/)
---

# Rechat (Painel Web)

##### Aplicativo simulador dispon�vel em [Rechat (APK)](https://breakdance.github.io/breakdance/)

--  
Rechat � uma ferramenta de coleta e processamento de dados para pesquisadores
interessados no estudo do comportamento de usu�rios em sistemas de bate-papo
m�vel, principalmente sobre aqueles expostos � conte�dos negativos. 

##### Funcionamento
Al�m do diagrama que apresenta o funcionamento e recursos, criamos um  [v�deo que explica na pr�tica](https://breakdance.github.io/breakdance/).

![Arquitetura de Funcionamento](https://raw.githubusercontent.com/ribaslucian/rails-chat-channel/master/public/rechat_arquitetura.jpg)


### Requisitos
* Servidor Web: Ruby (vers�o 2), Rails (vers�o 5), Python (vers�o 3)
* *Smartphone* Android 4.0+

### Instala��o
**Painel Web:**
1. Configure um servidor com os requisitos descritos.
2. Atrav�s de um terminal, fa�a clone do painel web (esse reposit�rio) e acesse seu diret�rio:

```sh
$ git clone https://github.com/ribaslucian/rails-chat-channel
$ cd rails-chat-channel
```

3. Prepare o ambiente l�gico do painel web gerando seu banco de dados e inserindo dados iniciais:
```sh
$ rails db:migrate db:seed
```

4. Inicie o servidor vinculando ao IP do host local a porta 3000 (voc� pode usar a porta que desejar):
```sh
$ rails s -b 0.0.0.0 -p 3000
```

5. Pelo navegador, teste o funcionamento acessando `localhost:3000` � a p�gina de acesso do Rechat deve ser exibida.


**Aplicativo:**
1. Baixe a APK do aplicativo nesse endere�o e instale em um celular.
Nota 1: Deve estar configurada a permiss�o para instalar de fontes desconhecidas.
Nota 2: O aplicativo deve estar na mesma rede que o painel.

2. Abra o aplicativo e fa�a a sincroniza��o com o painel, informando seu endere�o IP e a porta no menu "sincronizar com painel web": `IP_DO_HOST:3000`
3. Se aplicativo retornar uma mensagem verde e redirecionar para tela de acesso, tudo est� configurado.

### Utiliza��o
[V�deo Demonstrativo](https://breakdance.github.io/breakdance/)

[Artigo em PDF (ACM/Webmedia)](https://breakdance.github.io/breakdance/)

---
**Licen�a e Apoios**

<sup> [*Creative Commons* Atribui��o-N�oComercial-SemDeriva��es Internacional 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode}) 
Pesquisa intermediada pela Universidade Tecnologica Federal do Paran� (UTFPR), atrav�s do Programa de P�s-Gradua��o em Computa��o Aplicada (PPGCA). Apoiado parcialmente pelo projeto GoodWeb (processo \#2018/23011-1 da FAPESP), CAPES e empresa Emissora e Gerenciadora de Cart�es Brasil LTDA.
</sup>
