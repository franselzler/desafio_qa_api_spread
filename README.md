# Desafio Técnico – Testes de API (ViaCEP)

## Objetivo
Este repositório contém a execução do desafio técnico de QA, cujo objetivo foi validar o funcionamento de uma API pública por meio da definição e execução de casos de teste, bem como a geração dos artefatos solicitados.

## API utilizada
- API ViaCEP  
- URL base: https://viacep.com.br  
- Tipo: API pública para consulta de endereços a partir do CEP

## Estratégia de Testes
Foram definidos e executados testes funcionais de API, contemplando:
- Fluxo básico de sucesso
- Fluxos alternativos
- Fluxos de exceção (CEP inexistente e inválido)
- Validação da estrutura da resposta

Os testes foram executados manualmente utilizando o Postman, com base nos casos de teste previamente documentados.

## Ferramentas utilizadas
- Postman – criação e execução dos testes de API
- Newman – execução da collection via linha de comando e geração de relatório automatizado
- GitHub – versionamento e disponibilização dos artefatos

## 📂 Estrutura do repositório

```text
desafio-qa-api_spread
├── casos-de-teste
│   └── Casos_de_Teste_API_ViaCEP.docx
├── evidencias
│   ├── CT01_Consulta_CEP_Valido.png
│   ├── CT04_CEP_Inexistente.png
│   └── ...
├── postman
│   └── ViaCEP_Postman_Collection.json
├── relatorio
│   └── newman-run-report.html
└── README.md
```

## Relatório Final de Execução dos Testes
Todos os casos de teste definidos foram executados com sucesso.

| Caso de Teste | Descrição | Resultado |
|--------------|----------|-----------|
| CT01 | Consulta de CEP válido | Aprovado |
| CT02 | CEP válido com hífen | Aprovado |
| CT03 | CEP válido sem complemento | Aprovado |
| CT04 | CEP inexistente | Aprovado |
| CT05 | CEP com quantidade de dígitos inválida | Aprovado |
| CT06 | CEP com caracteres alfanuméricos | Aprovado |
| CT07 | Validação da estrutura da resposta | Aprovado |

Como etapa adicional, a collection do Postman foi executada via Newman, com geração de relatório automatizado em HTML, disponível na pasta `relatorio`.

## Observações finais
A API apresentou comportamento consistente com o esperado para todos os cenários testados, não sendo identificadas falhas funcionais durante a execução dos testes.
