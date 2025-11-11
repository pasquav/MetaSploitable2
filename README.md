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
  
## Configuradas as maquinas iremos iniciar os testes.
- Devemos acessar nossa maquina do metasploitable com o usuário e senha padrão msfadmin para descobrir o ip dela afim de sabermos o ip que iremos atacar.
- Após descoberto o ip vamos para nosso Kali abrir o terminal e acessar nosso Metasploit.
  - Para isso vamos acessar o terminal como root e usar o comando msfdb init para iniciar nossa base de dados
  - Agora dentro do metasploit vamos usar os seguintes comandos para obter informações sobre nossa maquina:
  -  db_nmap -sS 192.168.56.102  (IP do meu alvo)
   <img width="828" height="577" alt="image" src="https://github.com/user-attachments/assets/6d2282fd-0786-49cb-ba98-0a23af41d0b7" />

  -  db_nmap -sV 192.168.56.102
  <img width="805" height="628" alt="image" src="https://github.com/user-attachments/assets/04c4f22e-4ff6-4dfc-a81e-0ad956b1d3a4" />
  
  -  Com essas informações já saberemos as porta que iremos atacar e qual a versão dos softwares nessas portas
 
  -  Agora vamos abrir o msfconsole e pesquisar pela versão do ftp que iremos testar.
  - 
