
# Laboratório: Azure AI Search

🔗 [Acessar laboratório](https://aka.ms/ai900-ai-search)

Este laboratório demonstra como configurar uma solução de busca inteligente com o Azure AI Search, enriquecendo dados textuais com IA para proporcionar consultas mais inteligentes e contextuais.

---

## 🎯 Objetivo

Criar uma solução de mineração de conhecimento para descobrir insights a partir de avaliações de clientes usando **Azure AI Search**, **Azure AI Services** e **Storage Account**.

---

## 🛠️ Etapas

### 1. Criação dos Recursos

- **Azure AI Search**
  - Região: East US 2
  - Nome do Serviço: Único
  - Camada: Basic

- **Azure AI Services**
  - Região: mesma do AI Search
  - Camada: Standard S0

- **Storage Account**
  - Nome: único
  - Container: `coffee-reviews`
  - Região: East US 2

### 2. Upload dos Documentos

- Baixar os arquivos de avaliações de clientes.
- Criar container público `coffee-reviews` no Blob Storage.
- Realizar upload dos documentos extraídos para esse container.

### 3. Indexação e Enriquecimento

- Ir para o serviço Azure AI Search > "Import Data"
- Fonte de dados: container `coffee-reviews`
- Habilitar **habilidades cognitivas**:
  - Extração de frases-chave
  - Detecção de sentimentos
- Configurar campos do índice
- Executar indexador

### 4. Consulta no Índice

- Realizar buscas por palavras-chave no índice via portal.
- Observar os resultados com insights extraídos automaticamente.

---

## 💡 Insights

- O Azure AI Search, aliado às habilidades cognitivas, permite transformar dados não estruturados em informações pesquisáveis.
- Habilita funcionalidades poderosas para **chatbots**, **painéis analíticos**, **atendimento ao cliente**, entre outros.
- Indexadores podem ser configurados para executar automaticamente com novos dados.

---

## 📘 Aprendizados

- Importância de manter os recursos na mesma **região** e **grupo de recursos**.
- Como o enriquecimento automático com Azure AI Services eleva a qualidade da busca.
- Facilidade de uso do portal para configurar uma solução robusta sem necessidade de programação.

---

## 🧠 Aplicações Possíveis

- Buscas em **bases de conhecimento internas**
- Indexação de **documentos jurídicos**, **laudos médicos**, **avaliações de clientes**
- **Sistemas de recomendação** com base em sentimentos e entidades extraídas

---

## ✅ Conclusão

O Azure AI Search é uma ferramenta poderosa para análise de textos e construção de soluções de busca semântica com IA embarcada, podendo ser usado por desenvolvedores e analistas de dados com mínima intervenção de código.
