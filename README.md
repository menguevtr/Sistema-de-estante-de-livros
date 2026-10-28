# 📚 Sistema de Estante de Livros

Um sistema simples, feito em Python, para organizar uma estante de livros direto no terminal. Você cadastra os livros, consulta o que já tem guardado e o programa ainda avisa quando você tenta cadastrar um título repetido.

💬 Sobre o projeto

Esse projeto nasceu como um trabalho da faculdade, e a dinâmica foi bem interessante: outro grupo de alunos escreveu um briefing (o documento com o que o sistema precisava fazer) e o nosso grupo (Grupo 9) ficou responsável por transformar esse briefing em código.

Foi uma boa experiência de ver, na prática, como é receber um requisito de outra pessoa e ter que interpretar, planejar e entregar algo que funcione. Hoje ele está aqui no GitHub como parte do meu portfólio e como espaço para continuar aprendendo e evoluindo o código.

✨ O que ele faz
Cadastra livros com título e autor
Bloqueia títulos duplicados, sem diferenciar maiúsculas de minúsculas (então "Dom Casmurro" e "dom casmurro" são considerados o mesmo livro)
Lista todos os livros da estante
Avisa quando a estante está vazia
Não quebra com entradas inválidas: se alguém digitar uma letra no lugar de um número no menu, o programa só pede de novo
🚀 Como rodar

Você só precisa ter o Python 3 instalado. Não tem nenhuma biblioteca externa para instalar.

Clone o repositório:
bash
   git clone https://github.com/menguevtr/Sistema-de-estante-de-livros.git
Entre na pasta do projeto:
bash
   cd Sistema-de-estante-de-livros
Execute o programa:
bash
  estante-livros.py

Em alguns sistemas (Linux e macOS), o comando pode ser python3 estante.py.

Prefere não instalar nada? Você também pode copiar o código e rodar no Google Colab, que foi onde ele foi desenvolvido originalmente.

🖥️ Exemplo de uso
===== MENU =====
1 - Cadastrar livro
2 - Listar livros
3 - Sair
Escolha uma opção: 1
Digite o título do livro: Dom Casmurro
Digite o autor do livro: Machado de Assis
Livro 'Dom Casmurro' cadastrado com sucesso!

===== MENU =====
1 - Cadastrar livro
2 - Listar livros
3 - Sair
Escolha uma opção: 1
Digite o título do livro: dom casmurro
Digite o autor do livro: Machado de Assis
Opa! Já existe um livro com o título 'dom casmurro'. Cadastro recusado.

===== MENU =====
1 - Cadastrar livro
2 - Listar livros
3 - Sair
Escolha uma opção: 2

--- Livros da estante Minha Estante ---
- Dom Casmurro (Machado de Assis)
----------------------------------
🧩 Como o código está organizado

O projeto usa Programação Orientada a Objetos e tem duas classes principais:

Classe	Responsabilidade
Livro	Representa um livro, guardando o título e o autor. Também sabe se apresentar na tela.
Estante	Guarda uma lista de livros. É ela quem cadastra (verificando duplicados) e lista os livros.

Depois das classes, existe um menu em loop (while True) que conversa com o usuário e chama os métodos da estante, até a pessoa escolher a opção de sair.

O código está bem comentado de propósito, em linguagem simples, para que qualquer pessoa iniciante consiga ler e entender o raciocínio.

🎓 O que praticamos aqui
Classes, objetos e métodos
Listas e laços de repetição (for e while)
Condicionais (if, elif, else)
Validação de entrada do usuário (isdigit)
Comparação de textos ignorando maiúsculas e minúsculas (lower)
Leitura do briefing de outro grupo e tradução dele em código
🔭 Ideias para o futuro

Esse projeto é um ótimo campo de treino, e algumas melhorias que quero fazer com o tempo são:

 Remover um livro da estante
 Buscar livros por título ou autor
 Salvar os livros em um arquivo (JSON), para não perder tudo ao fechar o programa
 Marcar livros como "lido" ou "quero ler"
 Escrever testes automatizados
 Criar uma interface gráfica ou versão web
🤝 Contribuições

Sugestões, dicas e ideias são muito bem-vindas, principalmente porque estou aprendendo. Se quiser contribuir:

Faça um fork do projeto
Crie uma branch para a sua ideia (git checkout -b minha-melhoria)
Faça o commit (git commit -m "Descreve a melhoria")
Envie para o seu fork (git push origin minha-melhoria)
Abra um Pull Request

Ou, se preferir, é só abrir uma Issue contando o que você achou.

👤 Autor

GitHub: @menguevtr

Se esse projeto te ajudou de alguma forma, deixa uma ⭐ no repositório. Isso ajuda bastante e me motiva a continuar!
