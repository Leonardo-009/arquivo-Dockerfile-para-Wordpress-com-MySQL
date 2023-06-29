# arquivo-Dockerfile-para-Wordpress-com-MySQL

Podemos simular com vsCode ou um leito de codigo que você tenha, É importante ter Docker no Abiente que ira executalo, o Docker tem na versão linux e windows.

Utilizando Node.js criei uma imagem de uma API desenvolvida em Node.js.
Depois disso  eu utiliso o comando "npm init -y" para cria um arquivo package.json

![image](https://user-images.githubusercontent.com/88870830/168206952-510f2444-b19b-4867-92a6-93c73c8d328a.png)


logo em seguida crie um novo arquivo chamado index.js, dentro dele coloquei o código a baixo

![image](https://user-images.githubusercontent.com/88870830/168207284-5fee117a-c122-4c5d-a31b-0bab7c5c8bfa.png)

Bom, para que possa criar a imagem a partir da aplicação, irei  precisar criar dois novos arquivos o Dockerfile. Após a criação deles terei a seguinte estrutura:

![image](https://user-images.githubusercontent.com/88870830/168207869-2f57d551-f993-4964-99b2-120e7b226e13.png)

Agora para que possa criar a imagem, executei o comando a baixo no terminal dentro do diretório que eu criou o arquivo Dockerfile.
"docker build -t tadrianonet/nodeapi ."

Para verificar se ele executou corretamente, digite o comando a baixo no terminal:

![image](https://user-images.githubusercontent.com/88870830/168208577-3365a6fe-0329-4a69-ab73-57e99fb99971.png)

Agora para que possa criar o contêiner a partir da imagem que acabamos de criar, devemos executar o comando a baixo passando as portas que iremos utilizar:
"docker run -p 3000:8081 tadrianonet/nodeapi"

Abra o endereço <a target="_blank" href="http:127.0.0.1:30000"> localhost </a> no seu navegador para que possamos validar se os passos anteriores estão OK.
Assim devera aparece uma msn dizendo Olá!.

![image](https://user-images.githubusercontent.com/88870830/168209080-5562108e-3b9d-4b7d-af72-986a11f6aebe.png)

Utilizando o Wordpress com MySQL fiz um servido no Docker

![image](https://user-images.githubusercontent.com/88870830/168209229-9a5d9539-aabf-4e13-8e3f-4f3f442b19c5.png)

