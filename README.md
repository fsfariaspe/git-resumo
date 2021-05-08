Depois que criar o repositório no github, dentro do gerenciador de arquivos vá para dentro da pasta que contem os arquivos que quer enviar para o github, quando chegar lá, clica com o botão direito do mouse dentro da tela, não precisa ser em cima de nenhum arquivo, basta ser no meio da tela mesmo, vai abrir um menu de opções, daí selecione a opção "git bash here", vai abrir um terminal de linha de comando já dentro dessa mesma pasta, daí só é seguir a sequência abaixo:

1. Digita: **git init** + enter (para inicializar o git dentro da pasta).
   - Nesse momento o git cria uma branch ***master*** que você pode ver logo no final do endereço local da pasta.
   - Para mudar para a branch ***main*** que agora é a padrão do github, você só precisa digitar o seguinte: "git checkout -b main" isso cria a branch ***main*** e ao mesmo tempo já muda para dentro dela, confira no final do endereço local, vai aparecer (main).
   - Obs: Isso é para evitar a criação da branch ***master*** dentro do seu repositório no github.
2. Digita: **git config --global user.name "Seu nome"** + enter (para setar o seu nome no git).
   - Obs: Se você já fez isso, pode pular para o passo 3.
3. Digita: **git config --global user.email "seu@email.com"** + enter (para setar o seu e-mail no git).
   - Obs: Se você já fez isso, pode pular para o passo 4.
4. Digita: **git status** + enter (deverá aparecer um ou mais arquivos em vermelho, esses arquivos precisam ser adicionados no stage).
5. Digita: **git add nomedoarquivo.* ** + enter (para adicionar o arquivo a ser comitado) ou para adicionar todos os arquivos simplesmente digita "**git add .**" (coloca um ponto no final).
   - Depois disso, se você quiser dar um **git status** mais uma vez, vai perceber que o conteúdo que antes aparecia em vermelho, agora está aparecendo em verde, isso quer dizer que os arquivos estão prontos para serem comitados.
   - Obs: Se por acaso você modificar o arquivo depois que já tiver feito o **git add .** terá que repetir o passo 5.
6. Digita: **git commit -m "Sua mensagem" **+ enter (para empacotar o seu arquivo).
7. Digita: **git remote add origin https://github.com/endereco-do-github-completo** + enter.
8. Digita: **git push origin main** + enter (para empurrar o seu arquivo, ou arquivos para dentro do seu repositório remoto no github).

Pode ser que ele ainda te peça pra colocar o login e a senha se for a primeira vez, daí eu aconselho apertar o botão azul para o seu navegador fazer o login e depois que o login for bem sucedido, pode voltar lá no terminal que ele vai terminar de fazer o upload automaticamente, depois disso pode atualizar a página do repositório que o conteúdo vai estar lá.

Pronto, tá feito.