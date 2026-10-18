# Download Link Probe

Ferramenta de linha de comando para verificar links de download.

Ela identifica respostas bem-sucedidas, erros 404, redirecionamentos externos,
redirecionamentos internos e falhas de rede. O programa não baixa o arquivo:
ele apenas faz uma requisição de verificação.

## Uso

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python probe.py "https://exemplo.com/arquivo"
```

É possível verificar várias URLs na mesma execução:

```powershell
python probe.py "https://exemplo.com/a" "https://exemplo.com/b" --timeout 20
```

O script aceita URLs `http://` e `https://`. Caminhos locais de imagens não são
entradas válidas para esta ferramenta.
