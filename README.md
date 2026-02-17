# Detecção de Dados Sensíveis e Conformidade LGPD 🛡️

Este projeto foi desenvolvido como parte de um estudo prático sobre privacidade de dados, utilizando o **Google Colab** e a biblioteca **DataProfiler**. O objetivo principal é identificar automaticamente Informações de Identificação Pessoal (PII) em conjuntos de dados brutos, um passo essencial para a governança de dados e conformidade com a LGPD.

## 🚀 Tecnologias Utilizadas
* **Python 3.12**: Linguagem base para o processamento.
* **Pandas**: Biblioteca para manipulação e limpeza de estruturas de dados.
* **DataProfiler (ML)**: Ferramenta da Capital One para profiling e detecção de entidades sensíveis (E-mail, Telefone).
* **Regex & Custom Logic**: Implementação de lógica própria para detecção de nomes brasileiros e tratamento de partículas (stopwords).

## 📊 Funcionalidades do Projeto
* **Identificação Automática de PII**: Uso de Machine Learning para rotular colunas com e-mails e números de telefone.
* **Busca Customizada de Nomes**: Função desenvolvida para cruzar dados com dicionários de nomes e sobrenomes comuns, calculando a probabilidade de exposição de identidade por coluna.
* **Relatório de Diagnóstico**: Geração de um DataFrame consolidado com as predições de cada campo do dataset analisado.

## 🛠️ Desafios Técnicos Solucionados
Durante o desenvolvimento, enfrentei e resolvi conflitos críticos de dependências entre o ambiente padrão do Google Colab e as exigências do `DataProfiler`. A solução envolveu o controle manual de versões do **NumPy** e **TensorFlow**, garantindo a estabilidade da análise sem comprometer as funcionalidades de ML.

## 📂 Como Executar
1. Faça o upload do arquivo `Curso de privacidade 2.3.ipynb` para o seu Google Colab.
2. Certifique-se de carregar os arquivos de apoio na pasta lateral do ambiente:
   * `autoridades_navais.csv` (Dataset base)
   * `nomes_comuns.txt` & `sobrenomes_comuns.txt` (Dicionários de apoio)
3. Execute as células de instalação e importação conforme as instruções no notebook.
