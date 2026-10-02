# Design do site

O site antigo colocava todo o texto em painéis escuros por cima de uma maquete 3D. O texto ficava denso, a maquete perdia a forma de perto e as imagens da série nem apareciam. Esta versão foi refeita a partir de padrões que se repetem nos sites de narrativa mais premiados da web (vencedores do Awwwards e dos Webby, e reportagens interativas como *Snow Fall*, do NYT, e as do The Pudding).

## O que esses sites têm em comum, e onde isso está aqui

| Padrão | Exemplos de referência | Onde está no site |
|---|---|---|
| **Abertura com tensão**: preloader com contador e uma cortina que sobe | Lusion, Locomotive, Active Theory | contador de 0 a 100 e cortina que revela o título |
| **Rolagem que vira câmera**: a página é presa e a rolagem conduz a cena | páginas de produto da Apple, Igloo Inc. | a câmera atravessa o arco do Ó, e a frase de abertura se acende palavra por palavra |
| **Tipografia gigante revelada por máscara** | Obys, Cuberto, Dogstudio | todos os títulos entram palavra por palavra, de baixo para cima |
| **Troca de "luz" por capítulo** | Stripe Sessions, Bruno Simon | cada era tem uma paleta: papel (engenhos), fogo (1645), azul (1817), fumaça (usina), festa (1890) |
| **Galeria horizontal presa** | Resn, KPR, Porsche | "O mapa da viagem", com as 12 paradas |
| **Dado que se mexe com a rolagem** (*scrollytelling*) | The Pudding, NYT, Reuters Graphics | Batalha das Sedes, linha do tempo da usina, anel dos 199 dias, rota da fuga de 1817 |
| **Microinterações e cursor próprio** | Awwwards SOTD em geral | cursor com rótulo, botões magnéticos, cartões que inclinam, placas que viram |
| **Textura e movimento contínuo** | Messenger (Abeto), Prior Holdings | grão de filme, faixa de texto que reage à velocidade da rolagem, moenda girando |
| **Um conceito por tela** | Linear, Apple | cada capítulo abre com número, título e um resumo "Em uma frase" |

## Para ser didático

- **Os selos são ensinados antes de tudo** ("Como ler esta história"), com um exemplo de cada um. O quiz do capítulo 10 cobra exatamente isso.
- **"Em uma frase"** abre cada capítulo. Quem só passar os olhos sai sabendo o essencial.
- **Termos difíceis** (antífona, advento, arroba, tombamento, bumba meu boi…) têm definição ao passar o mouse ou tocar.
- **Números viram imagem**: 1 em cada 6 pessoas escravizadas vira uma grade de quadrados; os 199 dias viram um anel que se completa; as dez leis viram uma régua.
- **Esquemas, não ilustrações bonitas**: a moenda, a fuga de 1817 e a usina são desenhos simples, com legenda e a nota "esquema".
- **"Você sabia?"** separa as curiosidades do fio principal.

## Cuidados

- Funciona sem JavaScript (o conteúdo fica todo visível) e respeita `prefers-reduced-motion`.
- Layout próprio para celular, sem rolagem lateral.
- Os elementos interativos são botões de verdade, navegáveis pelo teclado, e os textos animados guardam um `aria-label` com a frase completa.
- O cursor próprio só aparece em mouse.
