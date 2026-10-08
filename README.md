# Calculadora Escolar

Aplicação estática para acompanhar notas, médias bimestrais, pontos anuais e projeções. Feita com HTML, CSS e JavaScript puro, sem backend ou conta de usuário.

## Como executar

Abra `index.html` em um navegador moderno. Para publicar, envie os quatro arquivos deste diretório para um repositório GitHub e habilite **Settings → Pages**, escolhendo a branch e a pasta que contém `index.html`.

## Regra escolar

Em **Configurações**, altere a média mínima, a pontuação anual necessária, a quantidade de períodos e a nota máxima. Os valores iniciais são média 7, nota máxima 10, quatro bimestres e meta de 28 pontos. A média atual considera somente os bimestres com avaliações cadastradas. Cada média bimestral usa a fórmula ponderada `soma(nota × peso) / soma(pesos)`; o peso padrão é 1.

## Dados e privacidade

Disciplinas, avaliações, pesos, configurações e preferência de tema são guardados no `localStorage` do navegador em uso. Os dados permanecem nesse dispositivo e não são enviados a servidor algum. Use **Exportar dados** para baixar uma cópia JSON, ou **Importar dados** para restaurá-la. Limpar os dados do navegador remove também o conteúdo salvo pela aplicação.

## Publicação no GitHub Pages

O site não precisa de build, Node.js, PHP ou banco de dados. A biblioteca Chart.js e as fontes são carregadas de CDNs; se esses serviços não estiverem disponíveis, a aplicação continua permitindo cadastrar e calcular notas, embora os gráficos e fontes externas possam não carregar. Coloque `index.html`, `style.css`, `script.js` e `README.md` na raiz publicada do repositório.
