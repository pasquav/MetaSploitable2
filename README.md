# MetaSploitable2
Repositório para fins didáticos utilizando 2 VM's a primeira com Kali linux e a segunda com o Metasploitable2 

1º Necessitamos do VirtualBox instalado em nossa máquina, ou algum virtualizador de sua preferência, eu utilizarei o virtualBox.
2º Devemos realizar o download dos arquivos para criarmos nossas maquinas, 
  - No site https://www.kali.org/get-kali/#kali-platforms conseguimos realizar o download da ISO do Kali linux, caso não saiba como fazer indico ver o vídeo https://www.youtube.com/watch?v=Tmo-koflFxw
  - No site https://www.rapid7.com/products/metasploit/metasploitable/ Conseguimos os arquivos para baixar o metasploitable2

3º Devemos criar a maquina vistual no VirtualBox, seguindo os passos:
  - Clicar em Novo
  - Colocar o nome da maquina e preencher os dados conforme a necessidade.<img width="961" height="820" alt="image" src="https://github.com/user-attachments/assets/0f9a361a-a9d7-4b94-8728-1926ba2fa20e" />
4º Após isso devemos criar nossa maquina com o metasploitable2
  - Clicar em Novo, porém agora vamos colocar o nome, depois vamos colocar o tipo da maquina virtual, escolha Debian, após isso vamos selecionar no campo disco rígido, utilizar disco rígido existente, procurar os arquivos do metasploitable2 que você realizou o download, e escolher o disco.
  - Após isso finalizar e partiremos para a configuração da rede.

5º Vamos configurar as redes das maquinas virtuais para que elas consigam se enxergar na rede sem que tenham acesso a internet para evitar problemas pois iremos trabalhar com uma maquina que está cheia de vulnerabilidades expostas.
  -Na maquina que queremos alterar vamos clicar com o botão direito e ir em configurações, depois em rede vamos deixar desta maneira. <img width="913" height="538" alt="image" src="https://github.com/user-attachments/assets/c9807870-fcf3-4dc2-b478-032b9b640e81" />
 
  -Notem que devemos fazer isto para ambas as maquinas, caso contrário não iremos enxergá-las na rede.
  
