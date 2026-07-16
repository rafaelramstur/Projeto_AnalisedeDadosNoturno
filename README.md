Para tornar o seu `README.md` interativo e dinâmico diretamente no GitHub, podemos usar alguns recursos visuais modernos, como **badges dinâmicos**, **detalhes expansíveis (dropdowns)** para organizar o conteúdo, **links rápidos de teste**, **tabelas interativas** e um **guia visual de como testar a API de forma simples**.

Aqui está uma versão otimizada e interativa do seu README:

---

```markdown
# 🚗 CarPrice Predictor API

<p align="center">
  <img src="https://img.shields.io/badge/Status-Online-brightgreen?style=for-the-badge" alt="Status">
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Flask-Framework-black?style=for-the-badge&logo=flask" alt="Flask">
  <img src="https://img.shields.io/badge/Scikit--Learn-Machine_Learning-orange?style=for-the-badge&logo=scikit-learn" alt="Scikit-Learn">
</p>

---

## 📌 Sobre o Projeto

Esta é uma API inteligente que estima o valor de mercado de um carro usado. O modelo de **Regressão Linear** analisa variáveis-chave e devolve uma estimativa de preço instantaneamente.

---

## 🗺️ Rotas Interativas (Como Testar)

Abra o seu terminal (ou ferramenta como Postman/Insomnia) e teste as rotas abaixo assim que o servidor estiver rodando!

### 🟢 1. Checar Status
* **Método:** `GET`
* **URL:** `http://localhost:8000/`

<details>
<summary><b>▶️ Clique aqui para ver a resposta esperada</b></summary>

```json
{
  "Autor": "Favaro",
  "Status": "API online e funcionando corretamente!"
}

```

---

### 🔵 2. Prever Preço do Veículo

* **Método:** `POST`
* **URL:** `http://localhost:8000/prever`
* **Body (JSON):**

```json
{
  "ano": 2020,
  "quilometragem": 35000,
  "motor": 1.0,
  "num_revisoes": 3
}

```

```json
{
  "Preço": 52450.32
}

```

---

## 🛠️ Experimente Localmente!

Siga os passos abaixo para colocar a API para rodar em menos de 2 minutos:

### 1. Preparação do Ambiente

```bash
# Clone o repositório
git clone [https://github.com/seu-usuario/nome-do-repositorio.git](https://github.com/seu-usuario/nome-do-repositorio.git)

# Entre na pasta
cd nome-do-repositorio

# Instale as bibliotecas necessárias
pip install flask flask-cors pandas scikit-learn

```

### 2. Inicialização

Certifique-se de que o arquivo `dataset_carros_usados.csv` está na pasta e execute:

```bash
python app.py

```

---

## 📊 Estrutura dos Dados Recebidos

O modelo utiliza as seguintes variáveis do seu arquivo `.csv`:

| Parâmetro | Tipo | Descrição | Exemplo |
| --- | --- | --- | --- |
| `ano` | `int` | Ano de fabricação do carro | `2018` |
| `quilometragem` | `int/float` | Quilômetros rodados | `50000` |
| `motor` | `float` | Potência do motor do veículo | `1.6` |
| `num_revisoes` | `int` | Quantidade de revisões feitas | `4` |

---

## 👤 Autor

Desenvolvido com 💻 por **Favaro**.

*Sinta-se à vontade para dar uma ⭐️ neste repositório se o projeto te ajudou!*

```

```