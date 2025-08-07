# Comandos-UBUNTU
Sudo: comando que concede privilégio de administrador

Apt: gerenciador de pacotes

Sudo apt update: atualiza a lista de pacotes disponíveis (só consulta, não instala nada)

Sudo apt upgrade: instala as atualizações disponíveis para os pacotes que você já tem

Sudo reboot: reinicia a maquina

Sudo apt install build-essential dkms linux-headers-$(uname -r)
Instala: build-essential: ferramenta para compilar código-fonte
dkms: recompilador de aplicações para compatibilidade com Kernel do convidado (guest)

cd /media/$USER/VBox_GAs_7.0.6
Caminha até o diretório onde está o aplicativo para instalar recursos adicionais de convidado
$USER é uma variável de ambiente que referencia o valor do usuário que está logado (nome de usuário)

sudo ./VBoxLinuxAdditions.run
Executa a aplicação disponível no diretório que acessou e instala os recursos

lsmod | grep vbox lsmod:
Lista módulos carregados no Kernel
grep: funciona como um filtro para pesquisar apenas as linhas que contenham o texto que deseja pesquisar (nesse caso, vbox)
vbox: prefixo que inicia normalmente os nomes dos módulos do VirtualBox
