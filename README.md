# Sistema NetPrime

Sistema web Flask do Ecossistema Prime / NetPrime.

## Rodar localmente

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

Acesse: http://127.0.0.1:5000

## Publicar no GitHub

```bash
git init
git add .
git commit -m "primeira versao sistema netprime"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/netprime-sistema.git
git push -u origin main
```

## Publicar no Render

1. Suba este projeto no GitHub.
2. No Render, crie um novo Web Service conectado ao repositório.
3. Build Command:

```bash
pip install -r requirements.txt
```

4. Start Command:

```bash
gunicorn app:app --bind 0.0.0.0:$PORT
```

## Atenção

As pastas `data/`, `uploads/` e `runtime/` não devem ser enviadas ao GitHub.
Elas podem conter dados internos, anexos, configurações e arquivos locais.
