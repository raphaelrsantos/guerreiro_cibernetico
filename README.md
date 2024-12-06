# guerreiro_cibernetico
Projeto da pós graduação de sistemas e agentes inteligentes da UFG 2024/25

# Passos para execução do script:
1. Instalar o python;
2. Caso não tenha criado, criar/ativar o ambiente virtual (.env);
3. Pelo terminal do VSCode, instalar o pacote uv: pip instal uv
4. Iniciar o pacote uv: uv init
5. Adicionar o pacote dotenv: uv add python-dotenv
6. Adiciona o pacote openai: uv add openai
   * Uma forma alternativa pode ser adicionando a linha "openai>=1.55.3" em "dependencies", no arquivo pyproject.toml e rodar o comando: uv sync
7. Cria uma arquivo .env e nele adiciona a chave API_KEY da openai:
   * Adicionar da seguinte forma: OPENAI_API_KEY="Digite aqui a chave";
8. Instalar a biblioteca Guardrails:
   * uv add guardrails-api-client==0.4.0a1
   * uv add guardrails-ai==0.6.0
9. Configurar o guardrails: guardrails configure
   Enable anonymous metrics reporting? [Y/n]: Y
   Do you wish to use remote inferencing? [Y/n]: n
   Caso ainda não tenha uma api_key, clique no link sugerido, faça o login, crie e copie a chave API do hub.guardrails;
   Cole a chave API Key apenas clicando com o botão direito no terminal e dê o enter;
10. Importe uma biblioteca guardrails desejada: guardrails hub install hub://guardrails/valid_url
11. Criar o arquivo guerreiro_cibernetico.py e inserir o código python;
12. Executar o código;
