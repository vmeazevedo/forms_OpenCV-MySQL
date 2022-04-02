# pyForms_OpenCV-MySQL
Aplicação de CRUD + reconhecimento facial diretamente da base de dados.

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

## Como rodar?
Quando o código for executado, será apresentado o menu abaixo com as opções de cadastro e identificação:
![image](https://user-images.githubusercontent.com/40063504/103282211-d6674d80-49b3-11eb-8b8c-84fc54b6c73f.png)

## Opção 1
Caso seja selecionada a opção 1, serão apresentados alguns campos para preenchimento do novo cadastro conforme demonstrado abaixo:
![image](https://user-images.githubusercontent.com/40063504/103282344-3bbb3e80-49b4-11eb-8720-9faa71b78780.png)


Após concluir o novo cadastro em nosso banco de dados, a tela de reconhecimento facial será apresentada.![image](https://user-images.githubusercontent.com/40063504/103282395-673e2900-49b4-11eb-8db4-0c012b900b25.png)

Nesta tela temos a opção de cadastrar uma nova foto de usuário (tecla de espaço), realizar o treinamento (letra t), ou sair (letra q). Apertando a tecla 'espaço' no teclado, vamos capturar as fotos para realizar o treino posteriormente.
![image](https://user-images.githubusercontent.com/40063504/103282503-c865fc80-49b4-11eb-877b-423246d026ce.png)

Ao pressionar 'espaço' será criada uma pasta chamada 'USUÁRIO' e dentro dela será criada uma pasta com o nome previamente cadastrado, dentro dessa pasta serão armazenadas todas as fotos do usuário que acabamos de cadastrar. No caso de um novo cadastro, outra pasta será criada automaticamente com o nome cadastrado dentro da pasta 'USUÁRIO'.
![image](https://user-images.githubusercontent.com/40063504/103282688-4fb37000-49b5-11eb-9497-9a6432d2c241.png)

Agora chegou a hora de realizar o treinamento do nosso algoritmo para que ele reconheça o usuário cadastrado através das fotos tiradas. Para fazer isso, pressione a tecla 't' na mesma tela em que fizemos a captura. O algoritmo será treinado e o nome do usuário cadastrado será apresentado diretamente na camada de reconhecimento facial.
![image](https://user-images.githubusercontent.com/40063504/103282855-c2245000-49b5-11eb-90b8-32ddf0cf4381.png)


## Opção 2
Quando o código for executado, será apresentado o menu abaixo com as opções de cadastro e identificação:
![image](https://user-images.githubusercontent.com/40063504/103282211-d6674d80-49b3-11eb-8b8c-84fc54b6c73f.png)

Se a opção 2 for selecionada, a tela de reconhecimento facial será apresentada ao usuário.![image](https://user-images.githubusercontent.com/40063504/103283063-5098d180-49b6-11eb-8bdb-1bf3fbd03b2d.png)

Como neste caso já temos nosso usuário cadastrado em nosso banco de dados na nuvem, bastará pressionar a tecla 't' para executar o algoritmo de treinamento para que ele reconheça o rosto do usuário e apresente seu nome.
![image](https://user-images.githubusercontent.com/40063504/103283159-88a01480-49b6-11eb-943f-748e6b21b0c8.png)

## Validando o registro via MySQL Workbench
Usamos o MySQL Workbench para validar que nosso usuário registrado foi registrado com sucesso![image](https://user-images.githubusercontent.com/40063504/103283248-c9982900-49b6-11eb-9211-f822b3fbb7fc.png)
