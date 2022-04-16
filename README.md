![pyForms_OpenCV-MySQL-removebg-preview](https://user-images.githubusercontent.com/40063504/163689382-1c041093-f22e-4a71-81bb-09541801fcb5.png)


# pyForms_OpenCV-MySQL
Aplicação CRUD + reconhecimento facial diretamente da base de dados.

![Supported Python Versions](https://img.shields.io/pypi/pyversions/rich/10.11.0) [![Twitter Follow](https://img.shields.io/twitter/follow/vmeazevedo.svg?style=social)](https://twitter.com/vmeazevedo) [![LinkedIn](https://img.shields.io/badge/LinkedIn-Vinícius_Azevedo%20-blue)](https://www.linkedin.com/in/vin%C3%ADcius-azevedo-45180ab2/)

![Star](https://img.shields.io/github/stars/vmeazevedo/pyForms_OpenCV-MySQL?style=social)
![Fork](https://img.shields.io/github/forks/vmeazevedo/pyForms_OpenCV-MySQL?label=Fork&style=social)

## Apoie esse projeto! 💵💵
Olá!
Você pode realizar doações de qualquer banco para minha chave Pix Itaú: **865875c7-c1cc-4254-8585-7c1616dfbc59**


## Requirements

```sh
pip install -r requirements.txt
```

## Exemplo de utilização

1. Clone o repositório para sua máquina

   ``
   git clone https://github.com/vmeazevedo/pyForms_OpenCV-MySQL
   ``
2. Execute o arquivo python ``app.py``.


## Como rodar?
Quando o código for executado, será apresentado o menu abaixo com as opções de cadastro e identificação:

![11](https://user-images.githubusercontent.com/40063504/161362069-5a17b388-2f65-43a9-adcf-7e6115bf8064.png)



## Opção 1
Caso seja selecionada a opção 1, serão apresentados alguns campos para preenchimento do novo cadastro conforme demonstrado abaixo:

![22](https://user-images.githubusercontent.com/40063504/161362076-7197fab8-5530-406c-bc4a-f0923dc09fb5.png)



Após concluir o novo cadastro em nosso banco de dados, a tela de reconhecimento facial será apresentada.

![1](https://user-images.githubusercontent.com/40063504/161358062-628c5636-a108-44f7-8f0e-6729e1ddc0c7.png)


Nesta tela temos a opção de cadastrar uma nova foto de usuário (tecla de espaço), realizar o treinamento (letra t), ou sair (letra q). Apertando a tecla 'espaço' no teclado, vamos capturar as fotos para realizar o treino posteriormente.

![3](https://user-images.githubusercontent.com/40063504/161358071-6748d55a-ae28-469d-937b-a56d09d3e565.png)


Ao pressionar 'espaço' será criada uma pasta chamada 'USUÁRIO' e dentro dela será criada uma pasta com o nome previamente cadastrado, dentro dessa pasta serão armazenadas todas as fotos do usuário que acabamos de cadastrar. No caso de um novo cadastro, outra pasta será criada automaticamente com o nome cadastrado dentro da pasta 'USUÁRIO'.
![7](https://user-images.githubusercontent.com/40063504/161358104-cccdb82a-6f55-4721-86f9-f2653eb928c9.png)


Agora chegou a hora de realizar o treinamento do nosso algoritmo para que ele reconheça o usuário cadastrado através das fotos tiradas. Para fazer isso, pressione a tecla 't' na mesma tela em que fizemos a captura. O algoritmo será treinado e o nome do usuário cadastrado será apresentado diretamente na camada de reconhecimento facial.
![4](https://user-images.githubusercontent.com/40063504/161358113-8de4afc5-505a-4a09-b0be-728457309f3b.png)



## Opção 2
Quando o código for executado, será apresentado o menu abaixo com as opções de cadastro e identificação:
![11](https://user-images.githubusercontent.com/40063504/161362086-a1e52a54-2a42-4bf2-a3e4-cf4e5f22c456.png)


Se a opção 2 for selecionada, a tela de reconhecimento facial será apresentada ao usuário.
![2](https://user-images.githubusercontent.com/40063504/161358203-38df2a8f-bd1d-46aa-b07b-5a502d12d3f1.png)


Como neste caso já temos nosso usuário cadastrado em nosso banco de dados, bastará pressionar a tecla 't' para executar o algoritmo de treinamento para que ele reconheça o rosto do usuário e apresente seu nome.
![5](https://user-images.githubusercontent.com/40063504/161358207-78de3f58-3937-467a-9a8b-69f56cb6435f.png)

![6](https://user-images.githubusercontent.com/40063504/161358214-eb1ab2f7-f100-436d-ae50-bfd57dc5534b.png)


## Validando o registro via MySQL Workbench
Usamos o MySQL Workbench para validar que nosso usuário registrado foi registrado com sucesso![image](https://user-images.githubusercontent.com/40063504/103283248-c9982900-49b6-11eb-9211-f822b3fbb7fc.png)
