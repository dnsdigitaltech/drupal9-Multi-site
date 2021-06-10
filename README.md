# Drupal 9 Multi-site e Criando um tema

1 - Crie dois diretórios onde ficara os seus sites na raiz ex: wonders, footballclub

2 - Dentro de drupal/sites crie os mesmos diretórios wonders, footballclub.

3 - Pego os conteúdos: default.services.yml, example.settings.local.php que está dentro de sites/default copie-os e cole-os dentro dos diretórios, footballclub criados, depois renomei os arrquivos para services.yml, settings.php detro de cada diretórios.

4 - Dentro de Sites crie um arquivo chamdo sites.php e coloque a seguinte linha de código referente ao seu domínio
    $sites = [
        'footballclub.lh' => 'footballclub',
        'wonders.lh' => 'wonders',
    ];

5 - Crie um link simbólico do Drupal para este diretórios wonders

    ln -s drupal footballclub

    ln -s drupal wonders

6 - Depois remova do diretótios criados conforme abaixo:
    rm -rf wonders
    rm -rf footballclub

7 - Agora vamos cria a imagem dos diretório conforme o exemplo abaixo:
    ln -s drupal footballclub
    ln -s drupal wonders

8 - Basta abrir os arquivos que serão diretórios conforme exemplo abaixo:
    cd footballclub
    cd wonders

9 - Está pronto e configurado basta acessar seus dominios e instalar/configurar a imagem do Drupal 9 com seus respectivos banco de dados.
    http://wonders.lh/
    http://footballclub.lh


