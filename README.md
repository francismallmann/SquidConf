# SquidConf
Controle de ACL do SQUID
Trabalho realizado para a disciplina de Segurança de Redes - UFSM

1. Instalação
apt-get install apache2
apt-get install php5
apt-get install squid3

Após a Instalação dos serviços básicos, copiar o conteudo deste diretório para
o caminho /var/www/html/

Copiar o arquivo squid.conf para o diretório /etc/squid3/

2. Estrutura
Arquivos .txt = Cadastros dos ranges das ACLs
Arquivos .html = Front-end
Arquivos .php = Back-end

2. Issues
Talves seja necessário dar permissão nos arquivos txt.
Após configurar uma ACL é necessário reiniciar o serviço do Squid, por algumas
restrições de segurança do Apache+PHP é complexo fazer pelo PHP.
É preciso configurar o arquivo /etc/sudoers colocando o usuário do apache,
 copiando o arquivo script para o diretório /usr/bin/ com permissão
(chmod 755 script).

Nome: Francis Mallmann Schappo
Mail: fschappo@inf.ufsm.br
