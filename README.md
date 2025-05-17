# Prototipo Detecção de Fake News

O projeto é uma tentativa inicial e bem simplificada de construir um detector de notícias falsas. A ideia central é pegar uma mensagem que o usuário digita e usar duas ferramentas poderosas do Google para tentar avaliar se ela pode ser fake news ou não.

Primeiro, ele usa o Gemini 2.0 Flash, que é um modelo de linguagem grande capaz de processar informações rapidamente. Pedimos ao Gemini para ler a mensagem e procurar por sinais de que ela já foi marcada como falsa, desmentida ou confirmada por fontes confiáveis.

Em segundo lugar, ele também utiliza a Pesquisa Personalizada do Google. Isso permite que o sistema faça uma busca rápida na internet por termos relacionados à mensagem do usuário, com foco em encontrar artigos de checagem de fatos ou notícias de fontes confiáveis que possam confirmar ou negar a alegação.

A "detecção" em si é bem básica: o código analisa as respostas do Gemini e os resultados da pesquisa por algumas palavras-chave. Se encontrar termos como "notícia falsa" ou links para sites de fact-checking, ele levanta um alerta.
