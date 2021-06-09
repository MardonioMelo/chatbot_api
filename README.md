# Chatbot_api
API para chatbot

## Arquivos de treino


Estilo do documento:

	1-instrução: |1
	2-instrução: Nome único desse arquivo sem caracteres especiais e inciado com letra ex: t_01_teste.
	3-instrução: |2
    4-instrução: Nome da intenção no máximo 3 palavras.
    5-instrução: |3
    6-instrução: O que o usuário pode dizer, no mínimo 3 exemplos, sendo cada exemplo em uma linha.
    7-instrução: |4
    8-instrução: Que bot vai responder, para resposta aleatórias escreva na próxima linha.
    9-instrução: |5

    * Use uma barra vertical '|' e um número de 1 a 5 nas instruções 1, 3, 5, 7 e 9. 
    * É possível incluir no mesmo arquivo mais de uma treinamento, basta reiniciar as instruções do n.1 a n.9.

## Teste NLP
- Informe no parâmetro message o texto "nlp" para modo de teste.
- O teste vai consultar os dados do arquivo treino/testing.json.
- Verifique o retorno da mensagem para analisar o resultado. 

## Iniciar servidor WebSocket do chat
> php server.php

## Testes Automatizados - PHPUnit
- Execute o comando para os testes automatizados com PHPUnit
> php vendor/bin/phpunit --testdox --color tests