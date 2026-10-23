# GPS 3D • Navegação

Primeira versão de uma aplicação web responsiva de mapa e navegação.

## Recursos incluídos
- Mapa interativo baseado em OpenStreetMap e MapLibre GL JS.
- Visualização inclinada (perspectiva 3D) e modo 2D.
- Solicitação de localização do aparelho pelo navegador, mediante permissão.
- Busca manual de destinos usando Nominatim.
- Atalho para abrir uma rota de carro no Google Maps.
- Interface adaptada para celular e desktop.

## Publicar com GitHub Pages
1. Abra Settings do repositório.
2. Entre em Pages.
3. Em Build and deployment, escolha Deploy from a branch.
4. Selecione a branch `main` e a pasta `/(root)`, depois Save.
5. Aguarde a publicação e abra o endereço informado pelo GitHub Pages.

## Limites importantes
- A perspectiva inclinada não significa que todos os edifícios e terrenos estarão modelados em 3D. Para relevo 3D e edifícios realistas, é necessário configurar fontes de dados compatíveis e respeitar seus termos.
- A camada de trânsito ao vivo está sinalizada como não configurada; não exibe condições inventadas. É necessário contratar/configurar um provedor que forneça dados de trânsito.
- O atalho de rota encaminha para o Google Maps. Esta primeira versão não calcula nem desenha rotas próprias no mapa.
- O GPS do navegador exige permissão e normalmente HTTPS; a precisão depende do aparelho, sinal e ambiente.
- A busca de lugares usa o serviço público Nominatim. Faça pesquisas somente por ação do usuário, evite automação/autocomplete e leia a política: https://operations.osmfoundation.org/policies/nominatim/
- O mapa público do OpenStreetMap tem políticas de uso e limites. Para produção com muitos usuários, configure um provedor de tiles apropriado.

## Tecnologias
- HTML, CSS e JavaScript
- MapLibre GL JS
- OpenStreetMap
- Nominatim
