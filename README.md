# Javascript-Rocketseat
Final exercises of each Rocketseat Javascript course module <a href="https://skylab.rocketseat.com.br/journey/starter" rel="nofollow">JavaScript Starter</a> 🖥️🚀

<h2>Exercícios Módulo 01 - Introdução JavaScript </h2>
<h3>Exercício #1</h3>
<p>Crie uma função que dado o objeto a seguir:</p>
<pre><code>var endereco = {
	rua: "Rua dos pinheiros",
	numero: 1293,
	bairro: "Centro",
	cidade: "São Paulo",
	uf: "SP"
};
</code></pre>
<p>Retorne o seguinte conteúdo:</p>
<p><code>O usuário mora em São Paulo / SP, no bairro Centro, na rua "Rua dos Pinheiros" com nº 1293.</code></p>

<h3>Exercício #2</h3>
<p>Crie uma função que dado um intervalo (entre x e y) exiba todos número pares:</p>
<pre><code>function pares(x, y) {
  // código aqui
}
pares(32, 321);
</code></pre>

<h3>Exercício #3</h3>
<p>Escreva uma função que verifique se o vetor de habilidades passado possui a habilidade "Javascript"
e retorna um booleano true/false caso exista ou não.</p>
<pre><code>function temHabilidade(skills) {
  // código aqui
}
var skills = ["Javascript", "ReactJS", "React Native"];
temHabilidade(skills); // true ou false
</code></pre>
<p><em>Dica: para verificar se um vetor contém um valor, utilize o método indexOf.</em></p>

<h3>Exercício #4</h3>
<p>Escreva uma função que dado um total de anos de estudo retorna o quão experiente o usuário é:</p>
<pre><code>function experiencia(anos) {
  // código aqui
}
var anosEstudo = 7;
experiencia(anosEstudo);
// De 0-1 ano: Iniciante
// De 1-3 anos: Intermediário
// De 3-6 anos: Avançado
// De 7 acima: Jedi Master
</code></pre>

<h3>Exercício #5</h3>
<p>Dado o seguinte vetor de objetos:</p>
<pre><code>var usuarios = [
{
nome: "Diego",
habilidades: ["Javascript", "ReactJS", "Redux"]
},
{
nome: "Gabriel",
habilidades: ["VueJS", "Ruby on Rails", "Elixir"]
}
];
</code></pre>
<p>Escreva uma função que produza o seguinte resultado:</p>
<p><code>O Diego possui as habilidades: Javascript, ReactJS, Redux O Gabriel possui as habilidades: VueJS, Ruby on Rails, Elixir</code></p>
<p><em>Dica: Para percorrer um vetor você deve utilizar a sintaxe for...of e para unir valores de um array
com um separador utilize o join.</em></p>


<h2>Exercícios: Módulo 02</h2>
<h3>Exercício #1</h3>
<p>Crie um botão que ao ser clicado cria um novo elemento em tela com a forma de um quadrado
vermelho com 100px de altura e largura. Sempre que o botão for clicado um novo quadrado deve
aparecer na tela.</p>

<h3>Exercício #2</h3>
<p>Utilizando o resultado do primeiro desafio, toda vez que o usuário passar o mouse por cima de
algum quadrado troque sua cor para uma cor aleatória gerada pela função abaixo:</p>
<pre><code>function getRandomColor() {
 var letters = "0123456789ABCDEF";
 var color = "#";
 for (var i = 0; i < 6; i++) {
 color += letters[Math.floor(Math.random() * 16)];
 }
 return color;
}
var newColor = getRandomColor(); // #E943F0
</code></pre>

<h3>Exercício #3</h3>
<p>A partir do seguinte vetor:</p>
<pre><code> var nomes = ["Diego", "Gabriel", "Lucas"]; </code></pre>
<p>Preencha uma lista ul no HTML com os itens da seguinte forma:</p>
<ul>
<li>Diego</li>
<li>Gabriel</li>
<li>Lucas</li>
</ul>

<h3>Exercício #4</h3>
<p>Seguindo o resultado do exercício anterior adicione um input em tela e um botão como a seguir:</p>
<pre><code>< input type="text" name="nome" />
< button onClick="add()" > Adicionar < /button >
</code></pre>
<p>Ao clicar no botão, a função adicionar() deve ser disparada adicionando um novo item a lista de
nomes baseado no nome preenchido no input e renderizando o novo item em tela juntos aos
demais itens anteriores. Além disso, o conteúdo do input deve ser apagado após o clique.</p>

<h2>Exercícios: Módulo 04</h2>
<h3>Exercício #1</h3>
<p>Crie uma função que recebe a idade de um usuário e retorna uma Promise que depois de 2
segundos retornará se usuário é maior ou não que 18 anos. Se o usuário ter mais que 18 anos de
idade o resultado deve cair no .then, caso contrário, no .catch</p>
<pre><code>function checaIdade(idade) {
 // Retornar uma promise
}
checaIdade(20)
 .then(function() {
 console.log("Maior que 18");
 })
 .catch(function() {
 console.log("Menor que 18");
 });
</code></pre>

<h3>Exercício #2</h3>
<p>Crie uma tela com um < input > que deve receber o nome de um usuário no Github. Após digitar o
nome do usuário e clicar no botão buscar a aplicação deve buscar pela API do Github (conforme
URL abaixo) os dados de repositórios do usuário e mostrá-los em tela:</p>
<p>URL de exemplo: https://api.github.com/users/diego3g/repos</p>
<p>Basta alterar "diego3g" pelo nome do usuário.</p>
<pre><code>< input type="text" name="user" />
< button onclick = "" >Adicionar< /button >
</code></pre>
<p>Depois de preencher o input e adicionar, a seguinte lista deve aparecer abaixo:</p>
<pre><code>< ul >
 < li >repo1< /li >
 < li >repo2< /li >
 < li >repo3< /li >
 < li >repo4< /li >
 < li >repo5< /li >
< /ul ></code></pre>

<h3>Exercício #3</h3>
<p>A partir do resultado do exemplo anterior adicione um indicador de carregamento em tela no lugar
da lista apenas enquanto a requisição estiver acontecendo:</p>
<pre><code>< li >Carregando...< /li >
</code></pre>
<p>Além disso, adicione uma mensagem de erro em tela caso o usuário no Github não exista.</p>
<p><em>Dica: Quando o usuário não existe, a requisição irá cair no .catch com código de erro 404.</em></p>

