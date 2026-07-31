Dashboard de Marketing — Área Incrível / Terrenistas

Dashboard interno do Grupo MNGT com dados de captação de leads, funil de qualificação comercial e desempenho de campanhas — Área Incrível e Terrenistas.

Acesso

O dashboard é publicado via GitHub Pages diretamente a partir deste repositório. Qualquer atualização no arquivo index.html (branch main) fica visível no link publicado em 1-2 minutos.

Estrutura
index.html — dashboard completo (HTML + CSS + JavaScript em um único arquivo, sem dependências externas de build)
README.md — este arquivo
Fonte de dados

O dashboard lê os dados diretamente da planilha do Google Sheets (Dashboard MNGT), via links de exportação CSV (/export?format=csv&gid=...). Não é necessário nenhum backend — a leitura acontece no navegador do usuário, a cada carregamento da página.

A planilha é alimentada por:

Webhook do GoHighLevel (GHL) → Google Apps Script (Code.gs, mantido separadamente na planilha) → abas Leads Diários / Funil Diário
Atualização manual (relatórios do Meta Ads) → abas Campanhas / Campanhas Diárias
Como atualizar o dashboard
Edita o arquivo index.html localmente ou direto pela interface do GitHub
Faz commit na branch main
Aguarda 1-2 minutos para o GitHub Pages republicar
Testa no link publicado com Ctrl+Shift+R (força ignorar cache do navegador)
Funcionalidades
Filtro por período (mês) ou por intervalo de datas exato (De/Até)
Funil de conversão completo, com etapas específicas por empresa
Comparativo com o mesmo período do mês anterior
Tabela de performance por campanha
Gráfico de CAC × ROI por empresa
Observações
Repositório deve permanecer público para o GitHub Pages funcionar no plano gratuito.
O link é acessível a qualquer pessoa que o tenha — não há autenticação. Não inclua dados sensíveis além do que já está na planilha de origem (que tem seu próprio controle de acesso via Google).
