# Guia rápido — Python, Jupyter e exploração de dados abertos

Este guia explica como preparar um ambiente básico para explorar dados abertos usando Python e notebooks Jupyter.

O objetivo é ter um ambiente simples e funcional para análise e visualização de dados para a oficina do Festival de Tecnologia Popular de Setúbal 2026.

---

# 1. Instalar Python

Python é a linguagem de programação que iremos utilizar.

## Download

Site oficial:

[https://www.python.org/downloads/](https://www.python.org/downloads/)

Recomendação:

* Instalar a versão mais recente do Python 3.

---

## Windows

Durante a instalação:

✅ Marcar a opção:

"Add Python to PATH"

Depois clicar em:

"Install Now"

---

## Linux

Muitas distribuições já incluem Python.

Verificar instalação:

```bash
python3 --version
```

Caso necessário:

### Ubuntu/Debian

```bash
sudo apt update
sudo apt install python3 python3-pip
```

---

## macOS

Recomendado instalar usando:

[https://brew.sh/](https://brew.sh/)

Depois:

```bash
brew install python
```

---

# 2. Verificar instalação

Abrir terminal / PowerShell e executar:

```bash
python --version
```

ou:

```bash
python3 --version
```

Deverá aparecer algo semelhante a:

```bash
Python 3.12.0
```

---

# 3. Instalar Jupyter Notebook

Jupyter permite criar notebooks interativos com:

* código
* texto
* gráficos
* visualizações

Instalação:

```bash
pip install notebook
```

ou:

```bash
pip3 install notebook
```

---

# 4. Instalar bibliotecas

## pandas

Biblioteca para manipulação e análise de dados.

```bash
pip install pandas
```

---


# 5. Executar Jupyter

No terminal:

```bash
jupyter notebook
```

---

# 6. Testar instalação

Criar um notebook novo e executar:

```python
import pandas as pd

print("Tudo funcionando!")
```

Se não aparecer nenhum erro, o ambiente está pronto.

---

# 7. Dados abertos de Lisboa

Portal Lisboa Aberta:

[https://lisboaaberta.cm-lisboa.pt/index.php/pt/](https://lisboaaberta.cm-lisboa.pt/index.php/pt/)

* [Anomalia da média anual da temperatura média
](https://dados.cm-lisboa.pt/dataset/anomalia-da-media-anual-da-temperatura-media/resource/cdea3998-b918-41fb-b161-09e3b296b890)
* [Monitorização de Parâmetros Ambientais da Cidade de Lisboa - Histórico 15/07/2021 a 15/01/2024](https://dados.cm-lisboa.pt/dataset/monitorizacao-de-parametros-ambientais-da-cidade-de-lisboa-historico-15-07-2021-a-15-01-2024
)
* [Condicionamentos de Trânsito](https://dadosabertos.cm-lisboa.pt/dataset/condicionamentos-de-transito
)

---

# 8. Ler um CSV com pandas

Exemplo:

```python
import pandas as pd

df = pd.read_csv("dados.csv")

print(df.head())
```

---


# Recursos úteis

## Documentação pandas

[https://pandas.pydata.org/docs/](https://pandas.pydata.org/docs/)

## Documentação Jupyter

[https://jupyter.org/](https://jupyter.org/)

## Tutorial Python

[https://docs.python.org/3/tutorial/](https://docs.python.org/3/tutorial/)
