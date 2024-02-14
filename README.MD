# Instalação do Newman
npm install -g newman

# Instalação do relátorio HTML para o Newman
npm install -g newman-reporter-htmlextra

# Execução
- Exportar no Postamn a coleção criada para um arquivo JSON
- Exportar as variáveis de ambiente e globais utilizadas para um arquivo JSON
- Adicionar os arquivos JSON exportador para a pasta do projeto no VSCode
- Definir o caminho de execução no package.json, em "scripts.test" passando as variáveis -e (para o arquivo de variáveis de ambientes) e -r para geração do relatório
- Exemplo: newman run ./pet-store-tests/pet-store-api.json -e ./pet-store-tests/variaveis-ambiente.json -r htmlextra
- Executar npm run test
- Relatórios serão gerados em HTML na pasta newman