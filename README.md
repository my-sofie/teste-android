![Sofie](https://mysofie.com/assets/images/logo.png)





# Teste de Android Developer Sofie

Seja bem vindo à seleção para a vaga de Android Developer da Sofie

Este desafio é usado para avaliar os seus quesitos técnicos.



### O Desafio

Seu objetivo é criar um app com duas telas seguindo o modelo abaixo: uma que exibe uma listagem de tarefas e outra que adiciona itens nesta listagem de tarefas atráves de uma API.



### Telas



![Tarefas](https://github.com/my-sofie/teste-android/blob/master/images/Tarefas.png)




![NovaTarefa](https://github.com/my-sofie/teste-android/blob/master/images/NovaTarefa.png)



Apenas a orientação vertical (Portrait) é necessária;

Temos o protótipo no Figma para visualizar melhor os componentes: [Developer/Android](https://www.figma.com/file/tj9EOuijFs5JZ3ZNNktLYD/Developer?node-id=0%3A1)



Ao acessar o link acima, clique no botão de comentário (formato de balão) para visualizar as dicas que foram deixadas em cada componente e deixe selecionado a página Android, conforme a figura abaixo

![FigmaTips](https://github.com/my-sofie/teste-android/blob/master/images/FigmaTips.png)



## Consumindo o serviço de tarefas

A API que realiza a listagem e a adição das tarefas se encontra publicada neste link [aqui](https://documenter.getpostman.com/view/11090068/Szf3YpTy?version=latest).

> Dicas: 
>
> - Todas as palavras que contém um sublinhado são um hiperlink que ajudará de alguma forma seu desenvolvimento deste app.
>
> - Neste link acima você encontrar a documentação da api, na **guia language** selecione **Java - [OkHttp](https://square.github.io/okhttp)**  (essa possivelmente será a sua principal biblioteca no app).



Abaixo seguem algumas informações sobre como utilizar esse serviço.



Listagem das tarefas

 - **URL**:  https://9g1borgfz0.execute-api.sa-east-1.amazonaws.com/beta/task

 - **Method**: GET

 - **QueryString**: opcional

```ini
email=sofie@sofie.com
```

 - **Response**
   
    ```json
    {
     tasks: [
       {
         "_id": "372efad7-9c69-4753-bf9b-ee7741aaed0c",
         "description": "lorem ipsum",
         "email": "sofie@sofie.com",
         "when": "2020-04-15T15:41:49.074693",
         "title": "tarefa 1"
       },
       {
         "_id": "15893f63-17b4-4ef3-bc69-019fda35c339",
         "description": "lorem ipsum",
         "email": "sofie@sofie.com",
         "when": "2020-04-15T15:39:19.126486",
         "title": "tarefa 2"
       }
     ] 
    }
    ```





Adicionar nova tarefa

 - **URL**:  https://9g1borgfz0.execute-api.sa-east-1.amazonaws.com/beta/task

 - **Method**: POST

 - **Headers**:

   ```ini
   Content-Type: "application/json"
   ```

 - **Body**:

   ```json
   {
     "title": "tarefa 2",
     "email": "sofie@sofie.com",
     "description": "lorem ipsum"
   }
   ```

 - **Response**

   ```json
   {
    "success": true,
    "data": {
      "_id": "15893f63-17b4-4ef3-bc69-019fda35c339",
      "description": "lorem ipsum",
      "email": "sofie@sofie.com",
      "when": "2020-04-15T15:39:19.126486",
      "title": "tarefa 2"
    } 
   }
   ```



### Pré-requisitos: 

 - [Versão mínima do SDK: 16](https://developer.android.com/about/dashboards);
 - [Utilização de bibliotecas de terceiros](https://developer.android.com/studio/build/dependencies?hl=pt-br);
 - Capricho nos tratamentos e validações dos campos;
 - Tela deve ajustar em devices de resolução pequena, acima de 4 polegadas.



### Diferenciais:

 - [Utilizar Kotlin](https://kotlinlang.org/docs/reference/android-overview.html);
 - [Android Jetpack](https://developer.android.com/jetpack);
 - [Utilização do git](https://guides.github.com/introduction/git-handbook/#basic-git).



### O que esperamos:

 - [Boa organização do código-fonte](https://developer.android.com/guide);
 - Boas práticas de Orientação a Objetos;
 - Tempo de entrega do app dentro do aceitável;
 - Código limpo e de fácil manutenção.





### Ao terminar o desafio:

- Caso o upload do projeto for feito no Github, envie o link para nós por e-mail: developer@mysofie.com com cópia para erik@mysofie.com

 
- Caso não tenha conta no Github, envie o zip do projeto para developer@mysofie.com com cópia para erik@mysofie.com


- Caso tenha vindo direto neste projeto a partir do Github, por favor, preencha o formulário de candidatura neste [link](https://forms.gle/TfyUHkLz5QJ2wb8U8), para que possamos fazer o retorno do contato.



Desejamos uma boa sorte!!

