# NOME DA DISCIPLINA — Site Quarto

Template de site Quarto para disciplina de graduação, no padrão usado no
Departamento de Botânica / Centro de Biociências, UFPE.

## Estrutura

```
.
├── _quarto.yml         # configuração do site (navbar, tema, output-dir)
├── custom.scss         # tema de cores (edite $primary para a cor do curso)
├── styles.css          # ajustes finos de CSS
├── index.qmd           # página inicial
├── syllabus.qmd        # ementa
├── schedule.qmd        # cronograma
├── assessment.qmd      # avaliação
├── sessions/           # uma página .qmd por semana/aula (listing automático)
├── slides/             # decks RevealJS correspondentes a cada aula
├── exercises/           # listas de exercícios
├── resources/           # links e recursos gerais
├── get-started/         # tutoriais de introdução ao R (1 a 5)
├── workbook/             # tutorial "monte seu próprio site"
├── img/                  # logos e imagens (adicione os arquivos, ver img/README.md)
└── data/                 # datasets usados nas aulas/exercícios
```

## Como usar

1. Edite `_quarto.yml`: título do site, cores, links de GitHub, footer.
2. Substitua os placeholders (NOME DA DISCIPLINA, CÓDIGO, NOME COMPLETO, e-mail, horário) em `index.qmd`.
3. Adicione as imagens em `img/` (ver `img/README.md`).
4. Duplique `sessions/week01.qmd` e `slides/week01-slides.qmd` para cada semana.
5. Prévia local:
   ```bash
   quarto preview
   ```
6. Publicar no GitHub Pages:
   ```bash
   quarto publish gh-pages
   ```
   (ou configure Actions para publicar a partir da pasta `docs/`)

## Licença

Sugestão: [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) para o conteúdo do curso.
