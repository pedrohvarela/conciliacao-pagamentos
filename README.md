## O problema

Dois arquivos descrevem os mesmos pagamentos:

- `asaas_export.csv` — vem do Asaas, a plataforma de pagamento. É gerado pelo sistema.
- `controle_interno.csv` — é preenchido à mão pelos funcionários da empresa.

As informações divergem porque uma base é automática e a outra é manual. E nem todos os
pagamentos passam pelo Asaas, então estar em apenas uma das bases nem sempre é erro.

Hoje eu bato as duas linha a linha, conferindo uma a uma se o registro está nos dois lados.
Sem essa conferência, cliente que já pagou recebe cobrança e cliente que deve passa batido.