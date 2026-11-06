# HRBA Interações Medicamentosas

**Ferramenta de suporte multiprofissional**  
Serviço de Traumatologia e Ortopedia – Hospital Regional do Baixo Amazonas (HRBA)  

Produto tecnológico do TCR de **Marco Antonio da Costa Ferreira**  
Programa de Residência Multiprofissional em Atenção Integral em Ortopedia e Traumatologia – UEPA (2026)  
Orientador: Prof. MSc. Christian Diniz Lima e Silva

**Demonstração:** [https://marco123gmod-dotcom.github.io/HRBA-intera-es/](https://marco123gmod-dotcom.github.io/HRBA-intera-es/)

---

## O que este protótipo entrega

| Recurso | Status |
|---------|--------|
| Checagem de interações com ≥ 2 medicamentos | ✅ |
| **Lista completa** de medicamentos da Padronização de Medicamentos do HRBA (≈298 princípios ativos) | ✅ |
| Classificação de gravidade (Contraindicado / Maior / Moderada / Menor) | ✅ |
| Contexto clínico específico de ortopedia/trauma | ✅ |
| Monitoramento, alternativas HRBA e manejo/reversão | ✅ |
| Lista oficial de MAVs – Sonoridade Semelhante (SS) + Medicamentos Potencialmente Perigosos (MPPs / Etiqueta Vermelha) | ✅ |
| Relatório para impressão / PDF | ✅ |
| Interface visual com abas e filtros por classe | ✅ |
| Código 100% estático, gratuito e pronto para intranet | ✅ |

---

## Como usar

1. Abra o arquivo `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).
2. Na aba **Checagem de Interações**:
   - Selecione 2 ou mais medicamentos (use o campo de busca ou os filtros de classe).
   - Clique em **Verificar Interações**.
   - Analise o resultado (gravidade, contexto ortopédico, monitoramento, alternativas e manejo).
   - Clique em **Relatório** ou **Imprimir / PDF** para gerar versão impressa.
3. Na aba **Medicamentos de Alta Vigilância (MAVs)**:
   - Consulte a lista oficial de sonoridade semelhante e de medicamentos potencialmente perigosos (etiqueta vermelha do Tasy), extraída do Manual de Padronização de Medicamentos do HRBA.
4. Na aba **Sobre o Projeto**: informações do TCR e próximos passos.

---

## Fonte dos dados de medicamentos

Todos os medicamentos listados na ferramenta foram extraídos do **Manual Institucional de Padronização de Medicamentos do HRBA** (versão 000 – 02/10/2023), incluindo:

- Classe terapêutica
- Código TASY
- Princípio ativo
- Nome comercial
- Apresentação e via
- Sinalização de Aparência Semelhante (AS)
- Lista 2.1 – Medicamentos com Sonoridade Semelhante (SS)
- Lista 2.2 – Medicamentos Potencialmente Perigosos (MPPs) com indicação de etiqueta vermelha

A ferramenta utiliza prioritariamente os nomes de princípio ativo e nome comercial padronizados no hospital.

---

## Como hospedar no servidor / intranet do HRBA

O protótipo é **100% estático** (apenas HTML + CSS + JavaScript). Não precisa de banco de dados, PHP, Node ou qualquer backend.

### Opção 1 – Servidor web interno (recomendado)
1. Copie a pasta do projeto para o servidor web do hospital (Apache, Nginx, IIS ou similar).
2. Exemplo de caminho: `http://intranet.hrba/interacoes/` ou `http://10.x.x.x/interacoes/`
3. Peça ao NTI para criar um atalho ou link na página inicial da intranet e nos computadores da Farmácia Satélite e postos de enfermagem.

### Opção 2 – Pasta compartilhada
1. Coloque a pasta em um diretório de rede acessível.
2. Os profissionais abrem o `index.html` diretamente pelo Windows Explorer ou criam um atalho na área de trabalho.

### Opção 3 – GitHub Pages / Netlify / Vercel (externo)
Útil para demonstração ou acesso remoto autorizado. O arquivo único funciona perfeitamente.

### Integração futura com Tasy
O NTI pode, em fase posterior, embutir a ferramenta em iframe ou criar um botão de atalho dentro do sistema Tasy apontando para a URL interna.

---

## Expansão futura (conforme TCR)

- Expandir a base de interações (hoje contém as prioritárias para o serviço de Traumato-Ortopedia).
- Manter sincronização com futuras revisões da Padronização de Medicamentos do HRBA.
- Versão PWA (instalável no celular).
- Treinamentos de 30 minutos por turno + QR Code impresso nos postos + vídeo tutorial de 3 minutos.
- Parceria com programadores voluntários da UEPA/UFOPA e NTI do HRBA.

---

## Fontes utilizadas

- Manual de Padronização de Medicamentos do HRBA (incluindo listas de MAVs)
- Conceitos de classificação Drugs.com / Micromedex®
- Bulas ANVISA e alertas ISMP
- Literatura de interações em pacientes ortopédicos e de trauma
- TCR de Marco Antonio da Costa Ferreira (2026)

---

## Aviso importante

Este é um **protótipo educacional e de suporte clínico**.  

Não substitui o julgamento clínico, consulta a bases pagas (Micromedex, Lexicomp) nem a avaliação do farmacêutico clínico do hospital.  
Sempre considere idade, função renal/hepática, comorbidades e procedimento cirúrgico do paciente.

---

**Santarém-PA • 2026**  
Código aberto • Gratuito • Adaptável • Baixo custo de manutenção
