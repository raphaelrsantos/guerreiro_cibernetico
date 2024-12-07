# site_seguro
Projeto para a disciplina de ePrompts, do curso de pós-graduação em sistemas e agentes inteligentes - UFG 2024/25. 
Trata-se de ferramenta que auxilia na avaliação do nível de risco associado a sites na internet além de de apoio à investigação de crimes cibernéticos e fraudes digitais.
Desenvolvido em colaboração pelos alunos Guilherme Lemes, Raphael Rodrigues e Thiago Santos.

# Passos para execução do script:
1. Instalar o python;
2. Caso não tenha criado, criar/ativar o ambiente virtual (.env);
3. Pelo terminal do VSCode, instalar o pacote uv: pip instal uv
4. Iniciar o pacote uv: uv init
5. Adicionar o pacote dotenv: uv add python-dotenv
6. Adiciona o pacote openai: uv add openai
   * Uma forma alternativa pode ser adicionando a linha "openai>=1.55.3" em "dependencies", no arquivo pyproject.toml e rodar o comando: uv sync
7. Cria uma arquivo .env e nele adiciona a chave API_KEY da openai:
   * Adicionar da seguinte forma: OPENAI_API_KEY="Digite aqui a chave"
8. Instalar a biblioteca Guardrails:
   * uv add guardrails-api-client==0.4.0a1
   * uv add guardrails-ai==0.6.0
9. Configurar o guardrails: guardrails configure
    * Enable anonymous metrics reporting? [Y/n]: Y
    * Do you wish to use remote inferencing? [Y/n]: n
    * Caso ainda não tenha uma api_key, clique no link sugerido, faça o login, crie e copie a chave API do hub.guardrails;
    * Cole a chave API Key apenas clicando com o botão direito no terminal e dê o enter;
10. Importe a biblioteca guardrails Valid URL: guardrails hub install hub://guardrails/valid_url
11. Importe a biblioteca guardrails Valid Json: guardrails hub install hub://guardrails/valid_json
12. Criar o arquivo python site_seguro.py e inserir o código python;
13. Executar o código;
