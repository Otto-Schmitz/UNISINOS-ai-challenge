# Desafio Deep Learning — Classificação Fashion-MNIST

Classificação de 10 categorias de vestuário com CNNs em TensorFlow/Keras.  
Três experimentos: Baseline, Dropout+BN, Data Augmentation.

## Pré-requisitos

- Python 3.10+
- CPU apenas (sem GPU necessária)

## Como rodar

```bash
# 1. Criar e ativar ambiente virtual
python3 -m venv venv
source venv/bin/activate          # Linux/Mac
# venv\Scripts\activate           # Windows

# 2. Instalar dependências
pip install -r requirements.txt

# 3. Registrar kernel Jupyter
python -m ipykernel install --user --name=venv --display-name "Python (venv)"

# 4. Abrir o notebook
jupyter lab desafio.ipynb
# ou
jupyter notebook desafio.ipynb
```

Selecione o kernel **"Python (venv)"** e execute todas as células (`Kernel > Restart & Run All`).

## Estrutura

```
.
├── desafio.ipynb          # Notebook principal (código + relatório)
├── requirements.txt       # Dependências com versões exatas
└── README.md              # Este arquivo
```

## Tempo estimado de execução

~15–25 minutos em CPU (3 modelos × 10–15 épocas, Fashion-MNIST 60k amostras).

## Dataset

Fashion-MNIST é carregado automaticamente via `keras.datasets.fashion_mnist` — sem download manual.
