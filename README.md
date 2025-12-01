# 📌 Retenção 5D — Aplicativo de Pesquisa de CPF  
Aplicativo desktop desenvolvido em **Python + PySide6** para realizar consultas de CPF, analisar ofertas personalizadas com base no `fx_score` e exibir informações relevantes do cliente.  
Inclui sistema de atualização de base, carregamento otimizado e interface aprimorada.

---

# ✨ Principais Funcionalidades

## 🔍 Pesquisa Inteligente de CPF
- Busca otimizada e responsiva  
- Filtragem automática para exibir **sempre a melhor conta** quando o cliente possui múltiplas  
- Mensagens claras para CPF inválido, inexistente ou base não carregada  

## ⚡ Carregamento Rápido & Otimizado
- Utiliza arquivo **Parquet** para leitura rápida  
- Otimização interna que reduziu significativamente o tempo de inicialização  

## 📊 Informações Detalhadas do Cliente
- Exibe desconto de farmácia  
- Mostra uso **total** e dos **últimos 3 meses**  
- Seleção automática da melhor conta disponível  

## 🔄 Atualização da Base (Modo restrito)
- Importação de novo arquivo Excel direto no app  
- Conversão automática para `dados.parquet`  
- Botão protegido por **código secreto** para evitar alterações indevidas  

---

# 🆕 Novidades Recentes

- Interface com cores mais modernas e agradáveis  
- Carregamento otimizado de dados  
- Lógica de busca revisada e mais precisa  
- Seleção inteligente da melhor conta ao cliente  
- Mensagens de erro e uso mais claras  

---

# 🗄️ Como funciona o banco de dados?

- O app utiliza **Parquet** como formato principal (rápido e leve)  
- Se não existir um `dados.parquet`:
  - O app cria uma base vazia  
  - Permite atualizar os dados via Excel  
- Pandas faz toda a manipulação, filtragem e geração da base  

---

# 🛠️ Tecnologias Utilizadas

- **Python 3.x**  
- **PySide6** — Interface gráfica (GUI)  
- **Pandas** — Manipulação de dados  
- **Parquet / Excel (XLSX)** — Fonte de dados  

---

# ▶️ Como Executar o Projeto

```bash
git clone https://github.com/JoaoGRSilva/Consulta_Parket
cd nome-do-projeto

pip install -r requirements.txt
python main.py
```
Caso não haja um arquivo dados.parquet, utilize a opção de atualizar a base via Excel.

---

# 🐞 Problemas Conhecidos

- Na primeira execução sem o arquivo dados.parquet, o app abrirá com a base vazia.
- É recomendado carregar um arquivo Excel através do menu de atualização.

---

# 🤝 Contribuições

Contribuições são bem-vindas!
Use issues para relatar bugs ou sugerir melhorias ou abra um pull request diretamente.

---

# 📄 Licença

Este projeto é licenciado sob a MIT License.

---

# 👨‍💻 Autor

Desenvolvido por João Gabriel Silva.
