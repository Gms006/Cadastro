📄 **Consulta e Atualização de Alvarás – Neto Contabilidade**

📌 ***Descrição***

Este script automatiza o processo de verificação e atualização dos status de alvarás e certidões nas pastas das empresas cadastradas. Ele identifica documentos por tipo e validade a partir do nome dos arquivos, preenche automaticamente uma planilha de controle e gera um relatório JSON com todos os resultados.

🧰 **Funcionalidades**

📂 Varredura de pastas de cada empresa para buscar documentos válidos (.pdf, .jpg, .png, .jpeg).

🔍 Identificação por tipo de documento: Alvará de Funcionamento, Bombeiros, Vigilância Sanitária, Licença Ambiental e Uso do Solo.

🕒 Extração da validade dos documentos diretamente do nome dos arquivos.

🧾 Preenchimento automático da planilha mestre (LISTA EMPRESAS - NETO CONTABILIDADE 2025.xlsm).

💾 Salvamento intermediário e final da planilha.

📊 Geração de relatório JSON com o status dos documentos por empresa.

🗂 **Estrutura Esperada das Pastas**

`G:\EMPRESAS\NOME DA EMPRESA\Societário\Alvarás e Certidões\[Nome do Município (opcional)]`

📋 **Pré-Requisitos**

Python 3.10+

xlwings

permissões para ler e escrever nas pastas da rede

arquivos de alvarás com padrão: `NOME - VAL dd-mm-aaaa`

🚀 **Como Executar**

Verifique se o caminho da planilha e da pasta de empresas está correto nas configurações.

Rode o script com:

`python consulta_alvarás.py`

🗃️ **Saídas**

Atualizações diretas na planilha Excel.

Arquivo status_alvaras.json contendo todos os dados processados por empresa.

📈 **Possíveis Melhorias Futuras**

Logs em arquivo (além do terminal).

Notificações por e-mail ou Telegram para alvarás vencidos.

Integração com banco de dados para armazenamento permanente.

🧠 **Autor**

Script desenvolvido e mantido por Maria Clara - Neto Contabilidade
