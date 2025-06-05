# Extração Automatizada de Dados de PDFs de Cabos Automotivos

## Visão Geral do Projeto

Este projeto tem como objetivo o estudo e a prática de técnicas de extração de dados estruturados e textuais de arquivos PDF. Utilizei técnicas de web scraping para baixar documentos técnicos e, em seguida, processei esses PDFs para extrair informações relevantes, organizando-as em formatos tabulares.

Inicialmete foi necessário a extração de especificações de 28 diferentes tipos de cabos automotivos do site [Eland Cables](https://www.elandcables.com/cables/flr-automotive-thin-wall-cable).

## Tecnologias Utilizadas

* **Python:** Linguagem de programação principal.
* **`requests`:** Para fazer requisições HTTP e baixar PDFs.
* **`BeautifulSoup4`:** Para parsear HTML e localizar URLs de PDFs.
* **`PyMuPDF` (fitz):** Para extração de texto de PDFs (informações descritivas).
* **`tabula-py`:** Para extração de tabelas de PDFs.
* **`pandas`:** Para manipulação, organização e armazenamento de dados tabulares (DataFrames e CSVs).
* **`re` (Regex):** Para padrões de busca e extração de texto específicos.
* **Google Colab:** Ambiente de desenvolvimento utilizado para execução e integração com o Google Drive.

## Estrutura do Repositório

* `notebooks/`: Contém os notebooks Jupyter (Google Colab) com o código-fonte executável.
    * `1_download_pdfs_webscraping.ipynb`: Script para baixar os PDFs do site da Eland Cables.
    * `2_extract_data_from_pdfs.ipynb`: Script para extrair dados textuais e tabelas dos PDFs baixados.
* `data/`: Armazena os dados brutos e processados.
    * `raw_pdfs/`: PDFs originais baixados do site.
    * `extracted_tables/`: Tabelas extraídas dos PDFs, salvas como arquivos CSV individuais.
    * `processed_data/`: Dados textuais consolidados de todos os PDFs em um único arquivo CSV.
* `src/`: Scripts Python refatorados para maior organização (opcional, mas recomendado para projetos maiores).
* `.gitignore`: Define arquivos e pastas a serem ignorados pelo Git (ex: arquivos temporários, `data/` grandes).
* `requirements.txt`: Lista das bibliotecas Python e suas versões, para replicar o ambiente.



