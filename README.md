# Site do Dr. Agenor Coldebella Filho

Site em um único arquivo (`index.html`) com os vídeos ao lado (`video-*.mp4`). Não precisa instalar nada.

## Arquivos
- `index.html`: o site.
- `video-pode.mp4`, `video-trombose.mp4`, `video-medicina.mp4`, `video-lifting.mp4`, `video-canetas.mp4`: vídeos dos reels (tocam dentro do próprio card ao tocar nele).
- `vercel.json`: configuração da Vercel.

Todos precisam ficar na MESMA pasta (a raiz do repositório).

## Onde trocar as informações
Abra o `index.html` no Bloco de Notas e procure por `const CFG`:
- `wa`: WhatsApp (somente números, com 55 e DDD).
- `address`: endereço.
- `coords`: `{ lat: -27.00000, lon: -50.00000 }` com as coordenadas do Google Maps (deixa o pino exato). Para pegar: abra o local no Google Maps, clique com o botão direito no ponto e clique nos números.
- `hours`: deixe `null` (atendimento combinado pelo WhatsApp).
- `ig` e `yt`: links do Instagram e do YouTube.
- `showResults`: `false` esconde a seção Resultados.
- Em `REELS`: título de cada card e o arquivo `video`. Para abrir um reel específico do Instagram ao tocar (cards sem vídeo), preencha `link`.
- Em `YT_VIDEOS`: vídeos do canal (título, duração, imagem e `link` opcional).

## Publicar com GitHub + Vercel
1. Crie um repositório vazio no GitHub (github.com > New repository).
2. Em **Add file > Upload files**, envie TODOS os arquivos deste zip (o `index.html`, os 5 vídeos `.mp4`, `vercel.json`, `.gitignore`, `README.md`). Clique em **Commit changes**.
3. Em vercel.com: **Add New > Project**, importe o repositório, em **Framework Preset** escolha **Other**, deixe **Build Command** e **Output Directory** em branco e clique em **Deploy**.

## Publicar sem GitHub
No computador, abra app.netlify.com/drop e arraste esta pasta (ou o zip).

## Para atualizar depois
Troque o arquivo no GitHub (Add file > Upload files) e dê Commit. A Vercel publica sozinha.
