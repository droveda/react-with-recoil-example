# React
* https://reactjs.org/docs/getting-started.html
* https://create-react-app.dev/docs/getting-started/
* npx create-react-app backend-and-react --template typescript --use-npm
* cd {pasta raiz do projeto}
* npm i
* npm start
* npm run build
* npm test

## Sobre hooks
* https://pt-br.reactjs.org/docs/hooks-rules.html
* Hooks são ótimos, pois nos ajudam a reaproveitar código e a simplificar componentes. Durante o curso, vamos conhecer alguns hooks do Recoil e até mesmo criar alguns customizados. Então, lembre-se sempre das regras dos hooks:
  * Apenas chame Hooks no nível mais alto. Não chame Hooks dentro de loops (for, foreach, while), condições (if, else if) ou funções aninhadas (por exemplo, numa função que é executada dado um evento de onClick).
  * Apenas chame Hooks a partir de componentes funcionais. Não chame Hooks a partir de funções comuns, fora de componentes React.

# Recoil (biblioteca para auxiliar no gerenciamento de estado)
* npm i recoil
* https://recoiljs.org/

## Recoil
* Criar atoms
  * exemplo: /src/state/atom.ts
* Acessar atoms
  * **useRecoilValue**
* Modificar atoms
  * **useSetRecoilState**
* Alternativa correta! Impecável. Seguindo a fonte de verdade, a documentação, o hook **useRecoilState** funciona da mesma forma que o useState, e nos retorna tanto o getter quanto o setter.
  * const [tamanhoDaFonte, setTamanhoDaFonte] = useRecoilState<number>(tamanhoDaFonteState)


## API Mock json-server
* https://github.com/typicode/json-server#getting-started
* npm install -g json-server
* criar/configurar o arquivo db.json
* json-server --watch db.json -p 8080
* http://localhost:8080/eventos

## Para deburar o estado com recoil
* https://recoiljs.org/docs/guides/dev-tools
* foi utiliado a primeira opcao: Observing All State Changes
