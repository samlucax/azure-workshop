# Objetivos do Workshop

- Mostrar o básico do funcionamento do Cypress
- Entender como integrar um Pipeline na Azure
  - Criar um novo projeto na Azure
  - Criar um novo Pipeline
  - Adicionar a importação do projeto do Github
  - Adicionar a tarefa de execução dos testes (Command Line)
  - Exibir o resultado dos testes na Azure (junit report)
  - O que mais é possível fazer na Azure
    - Cache das dependências do Cypress
    - Omitir download do binário do Cypress
    - Publicar artefatos do teste (relatório, imagens, vídeos)
    - Configuração via arquivos de YML (Pipeline scripts)
- Desafio pós-workshop
  - Escolher um item adicional e implementar, podem usar a cola como referência
  
[Cola aqui](http://test.com "Cola aqui")

## O que mais é possível fazer na Azure

**Cache das dependências do Cypress**
```yaml
# para windows o path é diferente
- task: CacheBeta@1
  inputs:
    key: cypress | $(Agent.OS) | package-lock.json
    path: /home/vsts/.cache/Cypress
    restoreKeys: cypress | $(Agent.OS) | package-lock.json
  displayName: Cache Cypress binary
```

**Publicar artefatos do teste (relatório, imagens, vídeos)**
```yaml

```


**Omitir download do binário do Cypress**
```

```# azure-workshop-cwi
