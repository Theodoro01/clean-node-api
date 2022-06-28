## Standard

Ultiliza o padrão standard que é: 

Não usa ; no final

Não deixa uma virgula sobrando no final do objeto

Usa aspas simples ao invés de duplas.

## lint-staged

Permite que a gente rode scripts na nossa staged area.

O que é Staged Area ?

Quando nós criamos um arquivo por exemplo e não add ele no git, ele esta fora da staged
area. Então que dizer que aquele arquivo não vai entrar no proximo commit.

Então o lint-staged permite eu rodas script somente nós arquivos que estão na staged area,
ou seja eu consigo fazer um tipo de validação nos arquivos que vão entrar no meu commit.

E isso é muito bom para impedimos commits que estão com o codigo mal formatado ou com problemas de teste.

  "lint-staged":{
    "*.js": [
      "standard"
    ]
  },

Sempre que ouver algum arquivo .js no nosso staged podemos verificar se ele está formatado corretamente.