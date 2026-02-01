# 📌 Gerador de QR Codes Patrimoniais – AGU Tocantins

Aplicação desktop desenvolvida em **Python** para **geração em lote de QR Codes** destinados à **identificação e controle de bens patrimoniais** da **Advocacia-Geral da União – AGU Tocantins**.

O sistema permite a leitura de arquivos **Excel (.xlsx)** ou **CSV (.csv)**, identifica automaticamente a coluna correta de patrimônio e gera QR Codes padronizados com identidade visual institucional.

---

## 🖥️ Interface

- Interface gráfica **moderna e responsiva**
- Tema **Dark / Light** com alternância em tempo real
- Layout seguindo boas práticas de **UX corporativo**
- Compatível com **Windows**
- Desenvolvido e testado com **Python 3.11**

---

## 🚀 Funcionalidades

### 📂 Importação de Dados
- Leitura de arquivos:
  - `.xlsx` (Excel)
  - `.csv`
- Detecção automática da coluna de patrimônio:
  - Prioriza **“Patrimônio novo”** (localizado nas 10 primeiras linhas)
  - Fallback para **“Patrimônio” / “Patrimonio”** no cabeçalho
- Tratamento automático de dados:
  - Ignora linhas vazias
  - Remove patrimônios duplicados
- Compatível com planilhas de diferentes estruturas

---

### 🔳 Geração de QR Codes
- Geração **em lote**
- Um QR Code por patrimônio
- QR Codes personalizados com:
  - Texto “Patrimônio Nº {código}”
  - Logo institucional como marca d’água
  - Layout em formato de cartão
- Arquivos gerados em **PNG**
- Pasta automática de saída:
```text
qrcodes_saida/

📊 Progresso e Monitoramento
Barra de progresso em tempo real

Contador de itens processados

Processamento em thread separada (interface sempre responsiva)

📝 Log de Processamento
Área de log integrada à interface
Menu de contexto (botão direito do mouse):

💾 Salvar log em .txt

📄 Exportar log para PDF
🧹 Limpar log

Logs incluem:

Data e hora
Status de cada patrimônio (OK / ERRO)

⚙️ Usabilidade Avançada

Menu superior:
Arquivo
Gerar QR Codes em Lote
Abrir Pasta de Saída
Ajuda
About (informações do sistema e do desenvolvedor)
Botão Gerar QR Codes em Lote fixo na interface
Rodapé clicável:
Abre o cliente de e-mail padrão para contato com o desenvolvedor

🎨 Tema (Dark / Light)

Alternância instantânea entre:
🌙 Dark (padrão)
☀️ Light
Controle via toggle no canto superior direito

📁 Estrutura do Projeto
agu-qrcode/

├── app.py              # Aplicação principal (GUI + processamento)
├── logo.png            # Logo institucional utilizado nos QR Codes
├── requirements.txt    # Dependências do projeto
└── README.md           # Documentação do projeto

🛠️ Requisitos
Python: 3.9 ou superior (recomendado 3.11)

Sistema Operacional:
Windows 10 ou superior

📦 Dependências
Todas as dependências necessárias estão listadas no arquivo requirements.txt.

📄 requirements.txt
customtkinter>=5.2.0
PyQRCode>=1.2.1
pypng>=0.20220715.0
Pillow>=10.0.0
openpyxl>=3.1.2
reportlab>=4.0.0
ℹ️ Bibliotecas como tkinter, csv, os, threading, datetime fazem parte da biblioteca padrão do Python e não precisam ser instaladas.

🔧 Instalação
Clone o repositório:

git clone https://github.com/seu-usuario/agu-qrcode.git
cd agu-qrcode
Crie e ative um ambiente virtual (opcional, porém recomendado):

python -m venv venv
venv\Scripts\activate
Instale as dependências:

python -m pip install --upgrade pip
pip install -r requirements.txt

▶️ Execução
Execute a aplicação com:

python app.py

📌 Observações Importantes
O arquivo logo.png deve estar no mesmo diretório do app.py
Patrimônios duplicados são removidos automaticamente
O envio de e-mail é realizado via cliente padrão do sistema (mailto:)
Aplicação ideal para uso institucional e administrativo

👨‍💻 Desenvolvedor
Maycon Douglas Oliveira da Silva
📧 E-mail: mayconwiner@gmail.com

📜 Licença
Projeto desenvolvido para fins institucionais e administrativos da
Advocacia-Geral da União – AGU Tocantins. e UEA - Unidade Estadual de Administração no Tocantins.

