## Criando uma conta GITHUB
### Para criar uma conta no GitHub, siga os passos abaixo:

1. Acesse o site github.com.
2. Clique em "Sign up" no canto superior direito e siga as instruções para criar sua conta.
3. Preencha os dados e finalize a criação da conta

## Criando um repositório
### Criar um repositório

1. No canto superior direito de qualquer página, selecione e clique em Novo repositório;
2. Digite um nome breve e memorável para o repositório. Por exemplo, "olá mundo";
3. Opcionalmente, adicione uma descrição do repositório. Por exemplo, “Meu primeiro repositório no GitHub";
4. Escolha uma visibilidade do repositório. (Publico, Privado);
5. Selecione Inicializar este repositório com um LEIAME;
6. Clique em Criar repositório.

## Baixando o repositório para maquina local
### Usando os primeiros comandos GIT;

1. Certifique-se que tem o git instalado na maquina, caso não instale o [GIT](https://git-scm.com/downloads/).
- Como testar: Execute o comando `git` em qualquer terminal desejado, caso informe que o comando não foi encontrado, significa que o mesmo não foi instalado!
2. Certifique que o GIT foi instalado com sucesso! Digite `git` no prompt de comando de sua preferência, deverá apresentar a sintaxe dos comandos git.
3. No github, no seu repositório criado, clique no botão `Clone` na aba `HTTPS` e copie o endereço que apresentará, como exemplo `https://github.com/xxx/xxx.git`.
4. Crie uma pasta de sua escolha na sua maquina, acesse o caminho dessa pasta no prompt de comando de sua escolha.
5. digite o comando:
```sh
git clone <endereço do repositório>
```
6. Pronto! Seu repositório foi baixado com sucesso!

## Fazendo alterações no projeto
Para alterar/incrementar seu projeto, voce pode utilizar qualquer editor de texto, mas eu aconselho utilizar um software gratuito, o [Visual Studio Code](https://code.visualstudio.com/download).
1. Após alterar o arquivo, sempre se salvar.
2. Voce tambem pode criar novos arquivos.

## Adicionando o(s) arquivo(s) para "lista" de arquivos desejados para o Commit.
### Aqui voce precisa informar ao git quais os arquivos voce deseja sinalizar para que possa ser "emcapsulado" para uma subida.

Antes disso, vmos saber quais arquivos foram alterados.
Podemos usar o comando git abaixo:
```sh
git status
```
Serão apresentados os arquivos que sofreram alteração.
para adicionar os arquivos alterados, usaremos o comando a seguir:

```sh
git add <nome do arquivo>
```
Após ser adicionado, voce poderá checar, usando o mesmo comando `git status`

## Realizando o primeiro Commit
### agora chegou a hora de "assinarmos" nossa alteração.
Para fazermos essa "assinatura" usaremos o comando a seguir:
```sh
git commit -m "Nome de que desejar para uma referencia"
EX: git commit -m "Meu primeiro commit"
``` 

Porém, algo aconteceu! Não foi possível subir as alterações, _porque precisamos informar o usuário e o e-mail_!
Após o erro é apresentado dois comandos para que possamos informar o nome do usuário e o e-mail. Essa ação ocorre apenas na primeira vez!
Lembra que falei que precisamos "assinar" o commit? é dessa forma que podemos validar quem realizou as alterações e mantemos todo o rastreio das alterações.
Os comandos são:
```sh
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@example.com" 
```
Agora sim, após isso podemos usar o comando `git commit` novamente!

## Subindo as alterações para repositório

Para subirmos essas alterações, precisaremos usar o comando a seguir:
```sh
git push
```
Verifique no repositório as diferenças!

## Conclusão
Nesta aula aprendemos o básico para subirmos nossa primeira alteração no Github! Parabéns!

## Exercícios

### Exercicio_01 (Minha Rotina): 
1. Crie um repositório com o nome que desejar;
2. Adicione o arquivo readme;
3. Crie outro arquivo com o nome `Rotina.txt`;
4. Escreva sua rotina diária;
5. Salve os arquivos;
6. Adicione os arquivos;
7. Comite os arquivos;
8. E promova a subida para o repositório;

### Exercicio_02 (Trocando uma lâmpada):
Faça o processo semelhante ao exercício 01, porém informando como você trocaria uma lâmpada;

Para deixar seus projetos mais interessantes, utilize o formato markdown. Segue alguns sites utilizando essa formatação:
- [dillinger.io](https://dillinger.io/)
- [Markdownlivepreview](https://markdownlivepreview.com/)
- [stackedit.io](https://stackedit.io/app#) ✨