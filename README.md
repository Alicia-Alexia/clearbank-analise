# Análise Financeira com Python - ClearBank 📊

## Descrição do Projeto
Projeto prático desenvolvido como desafio final para a disciplina de Análise de Dados e Inteligência de Negócios com IA. O objetivo principal deste projeto é processar o histórico mensal de transações de uma fintech fictícia (ClearBank), aplicando técnicas de limpeza, validação e análise de dados utilizando Python.

O script foi desenhado para lidar com dados imperfeitos, filtrando campos vazios, tipos incorretos e datas inválidas de forma silenciosa, garantindo a integridade da análise financeira.

### Funcionalidades Implementadas
- **Validação de Dados:** Leitura de arquivos `.csv` via módulo nativo do Python, com filtros de higienização de dados e tratamento de exceções (`try/except`).
- **Cálculo de Métricas:** Agrupamento de transações por mês para extração de totais de crédito/débito, saldo, médias e valores extremos.
- **Detecção de Anomalias:** Identificação automática de movimentações suspeitas com valores superiores a R$ 10.000,00.
- **Exportação de Dados:** Geração de um relatório consolidado em formato `.json`.
- **Visualização de Dados:** Integração com `pandas` e `matplotlib` para plotagem do saldo mensal em um gráfico de barras.

---

## 🚀 Como Executar

Este projeto foi construído no formato Jupyter Notebook. Siga os passos abaixo para testá-lo:

1. **Clone este repositório:**
   ```bash
   git clone [https://github.com/Alicia-Alexia/clearbank-analise.git](https://github.com/Alicia-Alexia/clearbank-analise.git)


2. **Abra o Notebook:**
* Faça o upload do arquivo `clearbank.ipynb` no **Google Colab** ou abra-o localmente em seu **Jupyter Notebook** / **VS Code**.


3. **Dados de Teste:**
* Certifique-se de que o arquivo de dados fictícios `transacoes.csv` esteja no mesmo diretório do notebook (ou atualize o caminho de leitura no script caso esteja usando o Google Drive no Colab).


4. **Execução:**
* No menu superior, clique em "Run All" (Rodar Tudo) ou execute as células sequencialmente em ordem, de cima para baixo.



---

## 📂 Saídas Geradas

Ao executar as células do notebook com sucesso, o projeto irá gerar as seguintes saídas:

1. **Relatório no Terminal:** Um painel formatado impresso diretamente no console, contendo estatísticas de limpeza do CSV, o relatório mensal detalhado (com formatação monetária padrão BRL) e a listagem de transações suspeitas bloqueadas.
2. **`relatorio.json`:** Arquivo exportado contendo as métricas de análise consolidadas e estruturadas.
3. **`grafico.png`:** Gráfico de barras salvo automaticamente demonstrando a variação do saldo (crédito x débito) ao longo dos meses analisados.

