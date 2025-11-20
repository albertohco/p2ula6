# Gerenciador Web de Eventos

Um projeto minimalista de gerenciador de eventos com arquitetura full-stack usando SQLAlchemy, FastAPI e Streamlit.

## Instalação

```bash
pip install -r requirements.txt
pip freeze -> lista_pacotes.txt
```

## Como Executar

### Terminal 1: Iniciar o Backend
```bash
uvicorn backend:app --reload
```

A API estará disponível em: http://localhost:8000/docs

### Terminal 2: Iniciar o Frontend
```bash
streamlit run frontend.py
```

O frontend estará disponível em: http://localhost:8501

## Estrutura

- **backend.py**: SQLAlchemy ORM, banco SQLite e API FastAPI
- **frontend.py**: Interface Streamlit
- **eventos.db**: Banco de dados SQLite (criado automaticamente)

## Endpoints da API

- `POST /eventos/` - Criar evento
- `GET /eventos/` - Listar eventos
- `GET /eventos/{evento_id}` - Obter evento
- `PUT /eventos/{evento_id}` - Atualizar evento
- `DELETE /eventos/{evento_id}` - Deletar evento

## banco de dados

```bash
sqlite3 eventos.db
```