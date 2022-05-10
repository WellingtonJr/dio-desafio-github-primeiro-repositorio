# Passo a passo git

## Link para download do Git
[Git download link](https://git-scm.com/download/win)

* Instalar git no pc windows/linux
* Criar/logar na conta github
* Gerar chave SSH:
    * Comando para criação da chave ssh(dentro do git bash): _ssh-keygen -t ed25519 -C "seuemail@email.com"_
    * Criar senha
    * Entrar no diretorio das chaves criadas: _/c/Users/"nomedousuario"/.ssh/_
    * LS para listar chaves(publica e privada)
    * Visualizar conteudo da chave publica(que será utilizada no github): _cat id_ed25519.pub_
    * Copiar chave pública
    * Colar em _Github > Settings > SSH Keys > New SSH key_
    * Gerar chave
    * Inicializar ssh agent(dentro do git bash): _eval $(ssh-agent -s)_
    * Entregar chave privada para o ssh agent: _ssh-add id_ed25519__
* Iniciar git em um diretorio "workspace":
    * Acessar seu diretório escolhido(pelo git bash) e usar o comando: _git init_
    * Configurar um nome e email para ser o autor dos seus futuros commits: _git config --global user.email "seuemail@email.com"_ e depois _git config --global user.name "SeuUsername(preferencialmente igual ao do GitHub)"_
* Commitas suas alterações(no gitbash, localmente):
    * Após realizar alterações no seu código ou diretórios, usar comandos:
        * _git add *_ (adiciona alterações a área Stage)
        * _git commit -m "mensagem explicando alterações do commit"_ (commita alterações)
        * _git status_ (verifica se está tudo ok).
* Criar novo repositório (dentro do github): 
    * _Perfil Github > Your repositories > New_
    * Gerar novo repositorio
    * Copiar endereço do repositorio gerado no GitHub
    * Abrir GitBash dentro do meu repositorio local
    * Apontar repositorio local(no GitBash) para repositorio remoto(GitHub) com o comando: _git remote add origin https://github.com/Usuario/exemplo.git_
    * _git status_ -> verifica se existe algum erro/pendência
    * _git push origin master_ -> envia modificações a nossa branch master remota
* Como resolver conflitos:
    * _git pull origin master_ -> pega alterações da branch master remota e efetua merge com minha branch local
    * Se houver conflitos, resolver conflitos localmente, apagar trechos (<< head === >>)
    * Salvar arquivos 
    * _git add *_ -> adiciona alterações a área Stage
    * _git commit -m "mensagem explicando alterações do commit"_ (commita alterações)
    * _git push origin master_ -> envia alterações para master remota
* Como clonar um repositorio GitHub:
    * Ir ao reposítorio escolhido
    * _Code > Copiar link do repositorio_
    * _git clone https://github.com/Urusario/exemplo.git_




