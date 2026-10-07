# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# Nome do projeto
- Cardio IA

## Nome do grupo
- Grupo 83

## 👨‍🎓 Integrantes: 
- Murilo Ferreira Borges - RM567738
- Guilherme Pinheiro Carlsson Cury - RM564011
- Estevão Ferreira Santos - RM567522

## 👩‍🏫 Professores:
### Tutor(a) 
- Leonardo Ruiz Orabona
### Coordenador(a)
- André Godoi Chiovato


## 📜 Descrição

O CardioIA é um projeto acadêmico desenvolvido com o objetivo de aplicar conceitos de Inteligência Artificial e Processamento de Linguagem Natural (PLN) na análise de relatos de pacientes.

O projeto é dividido em duas etapas. Na primeira, é utilizado um sistema baseado em regras que identifica sintomas presentes nos relatos dos pacientes e consulta um mapa de conhecimento para sugerir possíveis diagnósticos.

Na segunda etapa, é desenvolvido um classificador de texto utilizando Machine Learning. As frases são transformadas em representações numéricas por meio da técnica TF-IDF, e um modelo de Regressão Logística é treinado para classificá-las entre alto risco e baixo risco.

O projeto possui finalidade exclusivamente acadêmica e demonstra, de forma simplificada, como técnicas de IA podem ser aplicadas à análise de textos relacionados à saúde, não devendo ser utilizado para diagnóstico ou triagem médica real.


## 📁 Estrutura de pastas

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:

- <b>.github</b>: Nesta pasta ficarão os arquivos de configuração específicos do GitHub que ajudam a gerenciar e automatizar processos no repositório.

- <b>assets</b>: aqui estão os arquivos relacionados a elementos não-estruturados deste repositório, como imagens.

- <b>config</b>: Posicione aqui arquivos de configuração que são usados para definir parâmetros e ajustes do projeto.

- <b>document</b>: aqui estão todos os documentos do projeto que as atividades poderão pedir. Na subpasta "other", adicione documentos complementares e menos importantes.

- <b>scripts</b>: Posicione aqui scripts auxiliares para tarefas específicas do seu projeto. Exemplo: deploy, migrações de banco de dados, backups.

- <b>src</b>: Todo o código fonte criado para o desenvolvimento do projeto ao longo das 7 fases.

- <b>README.md</b>: arquivo que serve como guia e explicação geral sobre o projeto (o mesmo que você está lendo agora).

## 🔧 Como executar o código

### Pré-requisitos

Para executar o projeto, é necessário ter instalado:

- Python 3
- Jupyter Notebook
- pandas
- scikit-learn

As bibliotecas necessárias podem ser instaladas pelo terminal com:

```bash
pip install pandas scikit-learn notebook
```

### Estrutura utilizada

Os principais arquivos da Fase 2 estão organizados da seguinte forma:

```text
CardioIAfase2/
├── document/
│   ├── base_risco.csv
│   ├── frases_pacientes.txt
│   └── mapa_conhecimento.csv
│
├── src/
│   └── CardioIA_Fase2.ipynb
│
└── README.md
```

### Executando o projeto

1. Clone o repositório:

```bash
git clone URL_DO_REPOSITORIO
```

2. Acesse a pasta do projeto:

```bash
cd CardioIAfase2
```

3. Acesse a pasta `src`:

```bash
cd src
```

4. Inicie o Jupyter Notebook:

```bash
jupyter notebook
```

5. Abra o arquivo `CardioIA_Fase2.ipynb`.

6. Execute todas as células do notebook em ordem.

### Funcionamento

O notebook executa duas etapas principais:

**Parte 1 — Sistema baseado em regras:** carrega o mapa de conhecimento localizado em `document/mapa_conhecimento.csv`, analisa os relatos presentes em `document/frases_pacientes.txt` e sugere possíveis diagnósticos a partir das combinações de sintomas cadastradas.

**Parte 2 — Classificação com Machine Learning:** utiliza o arquivo `document/base_risco.csv` para treinar e testar um classificador de texto. As frases são transformadas em vetores utilizando TF-IDF e classificadas como `alto risco` ou `baixo risco` por um modelo de Regressão Logística.

Ao final, o notebook apresenta a acurácia, o relatório de classificação, a matriz de confusão e testes realizados com novas frases.

## Video

Segue link do video no Youtube como não listado: https://www.youtube.com/watch?v=70Cp8y9eVBc

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>


