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

## Como utilizar comandos no Robô
```
1 - execute o comando "ign gazebo [Modelo/Arena].sdf"
2 - Abra outro terminal e execute o comando "ign topic -e -t /keyboard/keypress"
3 - Após executar ambos, na simulação, ir nos 3 pontos e procurar/digitar "Key Publisher" e selecionar
4 - aperte em play
    4.1 - w = frente, a = esquerda, s = trás, d = direita, x = freio/parar.
```
