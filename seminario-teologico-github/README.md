# Seminário Teológico — site pessoal de estudos

Um ambiente de estudo responsivo em HTML, CSS e JavaScript puro, pensado para ser publicado no GitHub Pages. A interface foi inspirada em plataformas de ensino online, com identidade visual própria (azul-marinho, dourado, cartões de curso, trilha curricular e painel de progresso).

## O que já funciona
- Painel de progresso com 12 módulos e 48 etapas de aula.
- Grade curricular com filtros por categoria e aulas expansíveis.
- Páginas de aula com roteiro, passagens bíblicas, atividade e reflexão.
- Marcação de aulas concluídas.
- Biblioteca com atalhos para os PDFs locais.
- Caderno teológico com criação, edição, exclusão e exportação de anotações em Markdown.
- Rascunhos das atividades, reflexões e resultado de quiz.
- Tema claro/escuro.
- Busca básica no currículo.
- Progresso salvo no `localStorage` do navegador.

## Estrutura
```text
seminario-teologico/
├── index.html
├── styles.css
├── app.js
├── README.md
└── livros/
    └── README.txt
```

## Adicione seus PDFs
Copie os arquivos para a pasta `livros/` e use estes nomes (ou atualize os nomes no array `books` dentro de `app.js`):

1. `teologia-sistematica-eurico-bergsten.pdf`
2. `teologia-sistematica-pentecostal-stanley-horton.pdf`
3. `entendes-o-que-les-fee-stuart.pdf`

**Observação importante:** o PDF enviado com o título “Entendes o que lês?” aparenta ser um resumo atribuído ao Bookey, não necessariamente o livro integral. Confira o conteúdo e a edição antes de usá-lo como referência principal. O PDF de Teologia Sistemática Pentecostal também pode conter apenas parte do volume; confira o índice e a paginação.

Os PDFs não estão incluídos neste pacote de site. Adicione somente arquivos que você tem direito de armazenar e compartilhar no repositório. Se o repositório for público, considere manter os livros fora dele e estudar com cópias locais, respeitando direitos autorais.

## Visualizar localmente
Basta abrir `index.html` em um navegador moderno. Para melhor compatibilidade, você também pode executar um servidor local simples:
```bash
python -m http.server 8000
```
Depois abra `http://localhost:8000`.

## Publicar no GitHub Pages
1. Crie um repositório no GitHub.
2. Envie os arquivos e pastas desta estrutura.
3. No repositório, abra **Settings → Pages**.
4. Em “Build and deployment”, escolha **Deploy from a branch**.
5. Escolha `main` e `/ (root)` e salve.
6. Aguarde a publicação e abra a URL exibida pelo GitHub Pages.

## Dados e privacidade
O site não tem servidor nem login. Anotações, aulas concluídas, reflexões, rascunhos e preferências ficam no `localStorage` do navegador e dispositivo usados. Eles não são sincronizados automaticamente entre dispositivos ou navegadores. Use “Exportar anotações” para criar uma cópia do caderno em Markdown.

## Personalização
- Conteúdo curricular e livros: edite os arrays `modules` e `books` em `app.js`.
- Aparência: edite `styles.css`.
- Estrutura: edite `index.html`.

O conteúdo é um plano pessoal de estudos autodidata, não uma certificação nem uma equivalência acadêmica oficial.
