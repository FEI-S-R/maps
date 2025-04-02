# maps
## Observações
Os modelos foram desenvolvidos inicialmente utilizando o software Gazebo Fortress Simulator, estes modelos foram salvos na pasta "Modelos" enquanto os modelos desenvolvidos no Blender foram salvos no "ModelosBlender".  
### Modelos X ModelosBlender
Alguns modelos em Blender tiveram seus nomes alterados para melhor entendimento do usuário, sendo essas alterações:  
DexterityBox1 = Box  
DexterityBox2 = Box2  
DexterityBox3 = Box3  
DexterityRails = RailsW  
Os outros modelos desenvolvidos no Blender, continuam com os mesmos nomes.

## Como instalar Gazebo Fortress
* Versão utilizada de Linux  
```Ubuntu 22.04 Jammy```  
Primeiramente é necessário baixar algumas ferramentas necessárias
```
sudo apt-get update
sudo apt-get install lsb-release gnupg
```
Após instalar as ferramentas necessárias, baixe o Ignition Fortress  
```
sudo curl https://packages.osrfoundation.org/gazebo.gpg --output /usr/share/keyrings/pkgs-osrf-archive-keyring.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/pkgs-osrf-archive-keyring.gpg] http://packages.osrfoundation.org/gazebo/ubuntu-stable $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/gazebo-stable.list > /dev/null
sudo apt-get update
sudo apt-get install ignition-fortress
```
## Como desinstalar Gazebo Fortress
```
sudo apt remove ignition-fortress && sudo apt autoremove
```
## Como instalar Blender
* Versão utilizada
```Blender 3.0.1```
## Comandos para instalar o Blender
```
sudo apt update && sudo apt upgrade
sudo apt install blender
```
## Comandos para desinstalar o Blender
Remover o Blender  
```
sudo apt remove blender
```
Remover o Blender e suas dependências (Opcional)  
```
sudo apt autoremove blender
```
Remover o Blender e suas configurações (Opcional)  
```
sudo apt purge blender
```  

## Como utilizar comandos no Robô
```
1 - execute o comando "ign gazebo [Modelo/Arena].sdf"
2 - Abra outro terminal e execute o comando "ign topic -e -t /keyboard/keypress"
3 - Após executar ambos, na simulação, ir nos 3 pontos e procurar/digitar "Key Publisher" e selecionar
4 - aperte em play
    4.1 - w = frente, a = esquerda, s = trás, d = direita, x = freio/parar.
```
