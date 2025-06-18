# Organização e Pesquisa Inteligente de Documentos com IA

Este projeto documenta a aplicação das soluções Azure AI Document Intelligence e Azure Cognitive Search para armazenar, indexar e extrair informações relevantes de arquivos não estruturados.

---

## 1️⃣ Ingestão de Dados

- **Documentos utilizados:**  
  - `contrato_exemplo.pdf`  
  - `laudo_tecnico.docx`
- **Procedimento:**  
  Todos os arquivos foram caricados no **Azure Blob Storage** para facilitar o processamento pela IA.
- ![](images/upload_azure_blob.png)

---

## 2️⃣ Criação do Índice Inteligente

- **Ferramenta:**  
  Azure Cognitive Search conectado ao Blob Storage.
- **Configuração:**  
  Configurei o indexador para extrair campos, aplicar OCR e identificar entidades chave.
- ![](images/index_config_azure.png)

---

## 3️⃣ Exploração dos Dados Organizados

- **Consultas realizadas:**  
  - Buscar por termos específicos ("cláusula rescisória", "nome do responsável técnico")  
  - Consulta semântica por “responsabilidades do contratante”
- **Insights:**  
  - O OCR identificou textos em imagens do PDF.  
  - A IA reconheceu entidades como datas, nomes e valores monetários.
- ![](images/resultado_consulta.png)

---

## 💡 Resultados e Aprendizados

- **Valor percebido:**  
  - Rapidez na pesquisa por informação específica.  
  - Facilidade de identificar entidades complexas em documentos longos.
  - O processo é replicável para milhares de documentos.
- **Desafios:**  
  - Necessidade de revisar configurações do indexador para campos personalizados.
  - Validação manual de campos extraídos para evitar erros.

---

## 📷 Imagens das etapas

Consulte a pasta `/images` para ver prints do upload, configuração de índice e resultados das consultas.

---

## ▶️ Como executar

1. Faça upload dos arquivos de exemplo no seu Blob Storage.
2. Siga as etapas do README para indexação e busca na sua conta Azure.
3. Compare seus resultados com os documentados aqui.

---

> Repositório de desafio prático DIO. Para fins educacionais.
