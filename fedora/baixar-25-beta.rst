:Data: 15/Out/2016
Baixando e verificando a imagem do pré-lançamento do Fedora
============================================================

#. Acessar o página de divulgação dos pré-lançamentos: https://getfedora.org/en/server/prerelease/

#. Baixar a imagem do DVD do Fedora (arquivo .ISO): http://fedora.c3sl.ufpr.br/linux/releases/test/25_Beta/Server/x86_64/iso/Fedora-Server-netinst-x86_64-25_Beta-1.1.iso

#. Baixar arquivo contendo as somas de verificação (*checksum*, em Inglês): https://getfedora.org/static/checksums/Fedora-Server-25_Beta-1.1-x86_64-CHECKSUM

#. Calcular a soma de verificação da imagem de DVD::

  $ sha256sum Fedora-Server-netinst-x86_64-25_Beta-1.1.iso
  # Saída esperada:
  1786c1be417c9ba5f167c026c21979a6881d52ea6f2ac0851976d327d3d20ba8  Fedora-Server-netinst-x86_64-25_Beta-1.1.iso  
  
#. Comparar a soma obtida no passo anterior com a soma que aparece no arquivo de somas::

  $ cat Fedora-Server-25_Beta-1.1-x86_64-CHECKSUM
  # Saída (podada, por questão de simplicidade):
  [...]
  SHA256 (Fedora-Server-dvd-x86_64-25_Beta-1.1.iso) = eb3c9b54a0241df9fcd71a22896e962236465dec17ac6b88ebe4f8683066a95b
  SHA256 (Fedora-Server-netinst-x86_64-25_Beta-1.1.iso) = 1786c1be417c9ba5f167c026c21979a6881d52ea6f2ac0851976d327d3d20ba8
  [...]




