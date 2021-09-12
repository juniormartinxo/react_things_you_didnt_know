# ReactJS - Coisas que você não sabia do porque não leu a documentação:

### 1) Props possuem valor padrão “True”
Se você não passar nenhum valor para a prop, seu valor padrão será true. Essas duas expressões JSX são equivalentes:
```
<MyTextBox autocomplete />
<MyTextBox autocomplete={true} />
```

### 2) Atributos podem ser passado com spread `...`
Se você já tiver `props` como um objeto e quiser passar em JSX, você pode usar `...` como um operador “spread” para passar todo o objeto props. Esses dois componentes são equivalentes:
```
function App1() {
  return <Greeting firstName="Ben" lastName="Hector" />;
}

function App2() {
  const props = {firstName: 'Ben', lastName: 'Hector'};
  return <Greeting {...props} />;
}
```

### 
