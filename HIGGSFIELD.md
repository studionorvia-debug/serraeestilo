# Mídias do site — roteiro para o Higgsfield

O site procura estes arquivos na pasta `assets/`. Enquanto um arquivo não existir, aparece um painel escuro com as montanhas da logo e o número da peça — nada quebra.

**Já no site:** `peca-girafa.png`, `peca-cao.png`, `peca-atleta.png` (recortadas, **PNG sem fundo**) e a logo sem fundo (`logo-art.png` completa, `logo-mark.png` só as montanhas). `logo-original.png` (com o círculo preto) ficou só como ícone da aba do navegador.

**Regra do site:** imagem de peça em **`.png` com fundo transparente** aparece recortada, flutuando sobre o foco de luz com sombra no chão. Em **`.jpg`** aparece como foto inteira, ocupando o card. Para adicionar uma peça nova recortada, gere/recorte em PNG transparente e aponte o nome na lista `pieces` do `index.html`.

**Dica principal:** use as **fotos reais das peças** como *imagem de referência* no Higgsfield. Assim o cliente vê no site a peça que vai receber.

Estilo comum, no espírito da logo preto e branco (cole no fim de cada prompt):

> dark monochrome luxury editorial photography, deep black background, soft white rim light, subtle haze, high-end gallery catalog, shallow depth of field, ultra detailed, no text, no logo

---

## 1. Melhorar as 3 fotos que já estão no site (prioridade)

Os recortes foram feitos automaticamente a partir de prints do Instagram (baixa resolução, ~230–440px). Funcionam no tamanho do card, mas o ideal é:

1. **Fotografar de novo** (celular serve) com a peça inteira, fundo liso e boa luz, **ou** fazer **upscale 4×** das fotos originais no Higgsfield.
2. **Remover o fundo** (Higgsfield, remove.bg ou similar) e salvar como PNG transparente por cima de `peca-girafa.png`, `peca-cao.png`, `peca-atleta.png`.
   - No cão, a cabeça foi recortada à mão (havia uma mesa atrás) e o topo ficou levemente reto: uma foto nova resolve.

## 2. Vídeo do hero — `assets/hero.mp4` + `assets/hero.jpg`

- **Ferramenta:** Higgsfield Video (Kling / Veo / Seedance), image-to-video
- **Formato:** 16:9, 1080p, 6–10 s, **sem áudio**, loop. O site escurece o vídeo para o título branco ficar legível.
- **Imagem inicial (salve como `hero.jpg`):**
  > wide shot of a dark luxury showroom at night, black lacquered athlete sculpture on white marble, carved wooden giraffe in the shadows, black lacquered panther on a console, single soft white spotlight, polished floor reflections
- **Movimento:**
  > slow cinematic dolly-in, dust particles drifting in the light beam, reflections shimmer on the lacquer, very slow and smooth, seamless loop
- Mantenha o arquivo ≤ 6 MB.

## 3. Restante da coleção (4:5, 1600×2000)

| Arquivo | Peça (use a foto real como referência) | Prompt |
|---|---|---|
| `assets/peca-pantera.jpg` | Pantera preta laqueada | glossy black lacquered panther sculpture mid-stride, mirror-like reflections, low angle, dark stone plinth |
| `assets/peca-vaso.jpg` | Vaso-urna preto com medalhão | black lacquered urn vase on square pedestal with silver lion medallion, white flowers on top, centered |
| `assets/peca-pop.jpg` | Cão de balão vermelho / cães laqueados | glossy red balloon-dog style sculpture, automotive paint finish, on black marble, dramatic spotlight |
| `assets/peca-organica.jpg` | Escultura branca orgânica | white flowing organic sculpture of intertwined hands and waves, matte white, on dark console |
| `assets/peca-barroco.jpg` | Espelho barroco / mobília entalhada | ornate baroque gold-leaf mirror above a carved black console, candle glow, three-quarter view |

## 4. Showroom — `assets/showroom.jpg` (4:5)

Referência: foto real da loja (o post "Venha conhecer nossa loja") ou do tapete com a logo na entrada.
> interior of an intimate luxury decor boutique, curated sculptures on black pedestals, soft gallery spotlights, glass storefront at dusk, monochrome, inviting and exclusive

## 5. Bônus (Reels / anúncios)

Image-to-video de 6–10 s com órbita lenta de 30° em volta de cada escultura. Serve para Reels e pode substituir as fotos da coleção no futuro.

---

Depois de gerar, salve com o nome exato dentro de `assets/` e recarregue a página. Para trocar textos, nomes ou fotos das peças, edite a lista `pieces` no fim do `index.html`.
