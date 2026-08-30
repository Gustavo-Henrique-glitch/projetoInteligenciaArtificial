# projetoInteligenciaArtificial

# Diagnóstico de COVID-19, Pneumonia e Tuberculose via Raio-X

Projeto acadêmico de replicação e melhoria do artigo científico:

> Ahmed, M.S. et al. "Joint Diagnosis of Pneumonia, COVID-19, and Tuberculosis from Chest X-ray Images: A Deep Learning Approach." *Diagnostics*, 2023.

O artigo propõe uma rede neural convolucional (CNN) para classificar radiografias de tórax em 4 categorias: COVID-19, Normal, Pneumonia e Tuberculose. Este projeto replica o experimento original e, em seguida, propõe uma melhoria sobre o modelo.

## Como configurar o ambiente

### Pré-requisitos
- Python 3.10 a 3.13 instalado.
- As 3 bases de dados públicas baixadas (veja seção "Datasets utilizados" abaixo).

### Passo a passo

1. Clone este repositório e entre na pasta:
```bash
   git clone <url-do-repositorio>
   cd <nome-da-pasta>
```

2. Crie o ambiente virtual:
```bash
   python3 -m venv venv
```

3. Ative o ambiente virtual:

   **Linux/Mac:**
```bash
   source venv/bin/activate
```

   **Windows:**
```bash
   venv\Scripts\activate
```

4. Instale as bibliotecas necessárias:
```bash
   pip install -r requirements.txt
```

5. Configure os caminhos dos datasets na sua máquina:
```bash
   cp config.example.py config.py
```
   (no Windows, use `copy` em vez de `cp`)

   Depois, abra o arquivo `config.py` recém-criado e ajuste os caminhos (`RAIZ_COVID`, `RAIZ_PNEUMONIA`, `RAIZ_TUBERCULOSE`) para onde você salvou os datasets no seu computador.

6. Abra o Jupyter Notebook:
```bash
   jupyter notebook
```

## Datasets utilizados

- **COVID-19 Radiography Database** (Kaggle) — [link](https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database)
- **Chest X-Ray Images (Pneumonia)** (Kaggle) — [link](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- **Tuberculosis (TB) Chest X-ray Database** (IEEE DataPort) —[link](https://www.kaggle.com/datasets/tawsifurrahman/tuberculosis-tb-chest-xray-dataset)