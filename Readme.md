## Next Level Week Return </br>
--> 02/05/2022 </br> </br>

* Dia 01 Iniciando a Missão Impulse </br> </br>
  
1. Vamos precisar das seguintes ferramentas: </br>
  -> NodeJS(npm). </br> </br>
2. Começamos com a criação do projeto dentro da pasta especificada. </br>
   ```npm create vite@latest``` </br>
3. Escolher um nome para o projeto: "web" </br>
4. Selecionar o Framework: "react" </br>
5. Selecionar "react-ts" </br>
6. Apos a criação do projeto, navegamos para a pasta criada e iniciamos com o VSCode.</br>
   ```code .```</br>
7. Agora instalamos as dependencias com o código:</br>
   ```npm install```</br></br>

8. Vamos agora configurar o Tailwind.</br>
   ```npx tailwindcss init -p```</br>
9. Precisamos também adicionar a seguinte linha dentro do arquivo "tailwind.config.js".</br>
    ```content: ["./src/**/*.tsx"],```</br>
10. Instalar a seguinte dependencia:</br>
    ```npm install -D tailwindcss postcss autoprefixer```</br>
11. Vamos instalar a Biblioteca "Phosphor React", para podermos importar icones.</br>
    ```npm install phosphor-react```</br>
12. Vamos agora começar a falar sobre ACESSIBILIDADE.</br>
--> Código sem "Acessibilidade:
  ```import { ChatTeardropDots } from 'phosphor-react'```
    ```import { useState } from 'react'```
  ``````
    ```export function Widget() {```
      ```const [isWidgetOpen, setIsWidgetOpen] = useState(false)```
  ``````
  ```    function toggleWidgetVisibility() {```
        ```setIsWidgetOpen(!isWidgetOpen)```
  ```    }```
  ``````
      ```return (```
        ```<div className="absolute bottom-5 right-5">```
          ```{ isWidgetOpen && <p>Hello World</p> }```
  ``````
          ```<button onClick={toggleWidgetVisibility} className="bg-brand-500 rounded-full px-3 h-12 text-white flex items-center group">```
            ```<ChatTeardropDots className="w-6 h-6" />```
  ``````
            ```<span className="max-w-0 overflow-hidden group-hover:max-w-xs transition-all duration-500 ease-linear">```
              ```<span className="pl-2"></span>```
              ```Feedback```
            ```</span>```
          ```</button>```
        ```</div>```
      ```)```
    ```}```</br>
13. Vamos instalar a biblioteca( headless ) para utilizarmos acessibilidade.</br>
    ```npm install @headlessui/react```</br>

## 2° Dia Front-end da aplicação</br>
--> Continuando com o APP!</br>
1. Vamos aplicar uma cor de fundo diferente no corpo da aplicação atraves do global.css.</br>
2. Agora vamos criar um novo componete para abrirmos o formulario que vai conter as opções para o usuario.</br>
3. -> WidgetForm.tsx</br>
4. Apos a configuração do componente anterior, chegamos a conclusão que vamos precisar criar um novo componente para o nosso botão de fechar.</br>
5. -> CloseButton.tsx</br>
6. Fizemos algumas modificações no Componente WidgetForm.tsx.</br>
7. Continuar de 1:05:25 minutos de aula do Stage 2 no componente CloseButton.