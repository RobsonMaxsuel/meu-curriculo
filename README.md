# Conversor PDF → Markdown

Projeto para converter o PDF **Oracle_DBeaver_VirtualBox_Passo_a_Passo.pdf** em um arquivo Markdown.

## Pré-requisito

- **Python 3.8+** instalado. Se não tiver, baixe em [python.org](https://www.python.org/downloads/). Durante a instalação, marque a opção *Add Python to PATH*.

## Configuração (uma vez)

### 1. Criar o ambiente virtual (venv)

No PowerShell, na pasta do projeto:

```powershell
cd "c:\Users\Grande Papai\Downloads\Projeto CURSOR"
python -m venv venv
```

(Se o comando `python` não for reconhecido, use o caminho completo do seu Python, por exemplo:  
`C:\Python312\python.exe -m venv venv`.)

### 2. Ativar o venv

**PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

**Prompt de Comando (cmd):**

```cmd
venv\Scripts\activate.bat
```

Quando o venv estiver ativo, o prompt deve mostrar `(venv)` no início.

### 3. Instalar dependências

```powershell
pip install -r requirements.txt
```

## Uso

Com o venv ativado:

```powershell
python pdf_to_markdown.py
```

Isso converte o PDF padrão da pasta e gera **Oracle_DBeaver_VirtualBox_Passo_a_Passo.md** no mesmo diretório.

Para usar outro PDF ou outro arquivo de saída:

```powershell
python pdf_to_markdown.py "caminho\para\arquivo.pdf" "caminho\para\saida.md"
```

## Estrutura do projeto

- `venv/` – ambiente virtual Python (criado por você)
- `requirements.txt` – dependências (PyMuPDF)
- `pdf_to_markdown.py` – script de conversão
- `Oracle_DBeaver_VirtualBox_Passo_a_Passo.pdf` – PDF de entrada
- `Oracle_DBeaver_VirtualBox_Passo_a_Passo.md` – Markdown gerado
