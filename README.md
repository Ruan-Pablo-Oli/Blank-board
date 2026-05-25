# 🎨 Paint OpenGL

Aplicação de desenho vetorial interativo desenvolvida em **C com OpenGL/GLUT**, como trabalho da disciplina de Computação Gráfica da Universidade Federal do Cariri (UFCA).

## Funcionalidades

- Criação de objetos primários: ponto, segmento de reta e polígono
- Seleção e exclusão de objetos individuais
- Transformações geométricas: translação, rotação, escala, reflexão e cisalhamento
- Salvar e carregar objetos em arquivo
- Animação com objetos primários

## Dependências

- GCC
- OpenGL
- GLUT / freeglut

### Instalação das dependências

**Ubuntu / Debian:**
```bash
sudo apt update
sudo apt install gcc make freeglut3-dev libglu1-mesa-dev libgl1-mesa-dev
```

**Fedora / RHEL:**
```bash
sudo dnf install gcc make freeglut-devel mesa-libGLU-devel
```

**macOS (Homebrew):**
```bash
brew install freeglut
```

**Windows:**
Instale o [MinGW](https://www.mingw-w64.org/) e baixe as DLLs do freeglut em [freeglut.sourceforge.net](https://freeglut.sourceforge.net/).

## Como compilar

```bash
git clone https://github.com/seu-usuario/paint-opengl.git
cd paint-opengl
make
```

## Como executar

```bash
./paint
```

## Como usar

### Modos de operação

| Tecla | Modo |
|---|---|
| `P` | Desenhar ponto |
| `L` | Desenhar segmento de reta |
| `G` | Desenhar polígono |
| `S` | Selecionar objeto |

### Criação de objetos

| Objeto | Como criar |
|---|---|
| Ponto | Clique esquerdo na tela |
| Segmento de reta | Dois cliques esquerdos |
| Polígono | N cliques esquerdos + clique direito para fechar |

### Transformações (com objeto selecionado)

| Tecla | Transformação |
|---|---|
| Arrastar mouse | Transladar |
| `R` / `E` | Rotacionar sentido horário / anti-horário |
| `+` / `-` | Escalar para cima / para baixo |
| `X` | Reflexão em relação ao eixo X |
| `Y` | Reflexão em relação ao eixo Y |
| `O` | Reflexão em relação à origem |
| `H` | Cisalhamento horizontal |
| `V` | Cisalhamento vertical |
| `Delete` | Excluir objeto selecionado |

### Arquivo

| Tecla | Ação |
|---|---|
| `Ctrl + S` | Salvar objetos em arquivo |
| `Ctrl + O` | Carregar objetos de arquivo |

### Animação

| Tecla | Ação |
|---|---|
| `Espaço` | Iniciar / pausar animação |

## Estrutura do projeto

```
paint-opengl/
├── src/
│   ├── main.c
│   ├── objects.c
│   ├── selection.c
│   ├── transform.c
│   ├── fileio.c
│   ├── animation.c
│   └── ui.c
├── include/
│   ├── objects.h
│   ├── selection.h
│   ├── transform.h
│   ├── fileio.h
│   ├── animation.h
│   └── ui.h
├── docs/
├── Makefile
└── README.md
```

## Disciplina

**Computação Gráfica** — Curso de Ciência da Computação  
Universidade Federal do Cariri (UFCA)  
Professora: Luana Batista da Cruz

## Integrantes

<!-- Adicionar nomes aqui -->

---

> Trabalho acadêmico — entrega prevista para 21/06/2026.
