# DSX — Data Structures eXplorer

Plataforma interativa para visualização de estruturas de dados avançadas.

O DSX é uma aplicação web desenvolvida para auxiliar o aprendizado e a compreensão de estruturas de dados complexas por meio de visualizações interativas, execução passo a passo e acompanhamento dos estados intermediários dos algoritmos.

O projeto busca tornar visível o comportamento dinâmico de estruturas que normalmente são difíceis de compreender apenas por meio de implementações em código ou descrições teóricas, permitindo acompanhar como cada operação modifica a estrutura durante sua execução.

---

# Funcionalidades

## Árvore de Segmentos

Módulo de visualização interativa para árvores de segmentos, contemplando diferentes variantes da estrutura:

- Árvore de Segmentos Convencional;
- Lazy Propagation;
- Árvore de Segmentos Persistente.

Operações visualizadas:

- construção da árvore;
- consultas em intervalos;
- atualizações pontuais;
- atualizações em intervalos;
- criação e navegação entre versões persistentes.

A visualização permite acompanhar:

- nós visitados;
- nós modificados;
- propagação de valores pendentes;
- criação de novos nós em versões persistentes;
- compartilhamento de nós entre diferentes versões.

---

## Deque Monotônica

Módulo dedicado à visualização do algoritmo de janela deslizante utilizando Deque Monotônica.

O módulo permite acompanhar:

- inserção de elementos;
- remoção de elementos pelas extremidades;
- atualização da janela atual;
- manutenção da propriedade monotônica;
- evolução dos elementos armazenados durante a execução.

---

# Arquitetura

O DSX possui uma arquitetura modular, permitindo que diferentes estruturas de dados compartilhem mecanismos comuns de execução, gerenciamento de estados e visualização.

```

DSX
│
├── Módulos de Estruturas
│   │
│   ├── Árvore de Segmentos
│   │   ├── Convencional
│   │   ├── Lazy Propagation
│   │   └── Persistente
│   │
│   └── Deque Monotônica
│
├── Gerenciamento de Execução
│   ├── Registro de Estados
│   ├── Histórico de Execução
│   └── Controle de Passos
│
├── Camada de Visualização
│   ├── Renderização Gráfica
│   ├── Gerenciamento de Layout
│   └── Estados Visuais
│
└── Interface
├── Controles de Execução
├── Reprodução
└── Interação do Usuário

````

A arquitetura modular facilita a incorporação de novas estruturas de dados, permitindo reutilizar mecanismos existentes de:

- gerenciamento de estados;
- histórico de execução;
- animações;
- controles de interação;
- renderização.

---

# Sistema de Visualização

O DSX registra estados intermediários durante a execução dos algoritmos, permitindo observar não apenas o resultado final, mas também as etapas responsáveis pela transformação da estrutura.

Cada estado contém informações como:

- estrutura atual;
- operação realizada;
- elementos afetados;
- descrição da etapa executada.

O usuário pode:

- avançar e retroceder entre estados;
- reproduzir a execução automaticamente;
- pausar a animação;
- controlar a velocidade;
- analisar o comportamento da estrutura durante a execução.

---

# Tecnologias

- JavaScript
- HTML
- CSS
- Vite
- D3.js

---

# Executando localmente

Clone o repositório:

```bash
git clone https://github.com/emilsonfilho/DSX.git
````

Instale as dependências:

```bash
npm install
```

Execute o projeto:

```bash
npm run dev
```

Para gerar a versão de produção:

```bash
npm run build
```

---

# Estruturas Implementadas

| Estrutura                       | Status                |
| ------------------------------- | --------------------- |
| Árvore de Segmentos             | Implementada          |
| Lazy Propagation                | Implementada          |
| Árvore de Segmentos Persistente | Implementada          |
| Deque Monotônica                | Implementada          |
| Novas estruturas avançadas      | Arquitetura preparada |

---

# Objetivos do Projeto

O DSX tem como objetivo tornar estruturas de dados avançadas mais acessíveis por meio de uma abordagem visual e interativa.

O projeto busca apoiar:

* ensino de algoritmos;
* estudo de estruturas de dados;
* compreensão de execuções passo a passo;
* desenvolvimento de novos módulos de visualização.

---

# Trabalhos Futuros

Possíveis extensões incluem:

* inclusão de novas estruturas de dados avançadas;
* expansão dos recursos de explicação dos algoritmos;
* novos modos de visualização;
* ampliação da plataforma para contemplar diferentes algoritmos e estruturas.

---
