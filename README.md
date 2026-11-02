# HRBA Interações Medicamentosas – Protótipo Completo

**Ferramenta de suporte à equipe multiprofissional**  
Serviço de Traumatologia e Ortopedia – Hospital Regional do Baixo Amazonas (HRBA)  
Baseado no TCR de **Marco Antonio da Costa Ferreira** (Residência Multiprofissional UEPA – 2026)  
Orientador: Prof. MSc. Christian Diniz Lima e Silva

---

## O que este protótipo entrega

| Recurso | Status |
|---------|--------|
| Checagem de interações com ≥ 2 medicamentos | ✅ |
| Medicamentos padronizados do HRBA (foco Traumato-Ortopedia) | ✅ |
| Classificação de gravidade (Contraindicado / Maior / Moderada / Menor) | ✅ |
| Contexto clínico específico de ortopedia/trauma | ✅ |
| Monitoramento, alternativas HRBA e manejo/reversão | ✅ |
| Lista completa de MAVs (Sonoridade Semelhante + Potencialmente Perigosos) | ✅ |
| Relatório para impressão / PDF | ✅ |
| Interface visual com abas e filtros por classe | ✅ |
| Código estático, gratuito e pronto para intranet | ✅ |

---

## Como usar

1. Abra o arquivo `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).
2. Na aba **Checagem de Interações**:
   - Selecione 2 ou mais medicamentos (use o filtro ou os botões de classe).
   - Clique em **Verificar Interações**.
   - Analise o resultado (gravidade, contexto ortopédico, monitoramento, alternativas e manejo).
   - Clique em **Relatório** ou **Imprimir / PDF** para gerar versão impressa.
3. Na aba **Medicamentos de Alta Vigilância (MAVs)**:
   - Consulte a lista oficial de sonoridade semelhante e de medicamentos potencialmente perigosos (etiqueta vermelha do Tasy).
4. Na aba **Sobre o Projeto**: informações do TCR e próximos passos.

---

## Como hospedar no servidor / intranet do HRBA

O protótipo é **100% estático** (apenas HTML + CSS + JavaScript). Não precisa de banco de dados, PHP, Node ou qualquer backend.

### Opção 1 – Servidor web interno (recomendado)
1. Copie a pasta `hrba-interacoes` para o servidor web do hospital (Apache, Nginx, IIS ou similar).
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

- Aumentar a base de interações (hoje contém as prioritárias para o serviço).
- Adicionar mais medicamentos da padronização completa.
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

---

**Santarém-PA • 2026**  
Código aberto • Gratuito • Adaptável • Baixo custo de manutenção
