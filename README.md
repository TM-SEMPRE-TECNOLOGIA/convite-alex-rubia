# Convite de Casamento — Alex & Rúbia

Reclone do convite interativo `webgencyinvitations.com/thesacredgarden`
("The Sacred Garden" — Tilda), atualizado para o cliente.

## Dados do cliente
| Item | Valor |
|---|---|
| Noivos | Alex e Rúbia |
| Data/Horário | 27/09/2026 · 14h |
| Local | Praia de Maracaípe — em frente à Pousada Maraoka (Ipojuca, PE) |
| Paleta | Verde oliva + branco |
| RSVP | WhatsApp +55 81 8216-5064 |

## Estrutura
```
Alex e Rúbia - Convite Casamento/
├── index.html                        ← SITE (abrir este)
├── 01-ANATOMIA-TRANSICAO.md          ← Investigação da transição capa→vídeo→tela
├── 02-PROMPT-CAPA.md                 ← Prompt p/ gerar a arte da capa (iniciais + selo)
├── index-original-backup.html        ← Original Tilda (pasta webgencyinvitations.com)
├── The Sacred Garden (...) - singlefile-backup.html  ← Original SingleFile completo
└── assets/
    ├── video-abertura.mp4            ← Vídeo 4.8s com a foto do casal (ken burns)
    ├── musica.mp3                    ← Música de fundo (Einaudi — placeholder)
    ├── casal.webp / casal.jpg        ← Foto otimizada (900px, 265KB/311KB)
    ├── foto-casal-original.png       ← Foto original (8MB, backup)
    ├── referencia-capa-original.png  ← Capa do convite original (referência)
    └── fonts/                        ← Cinzel, Ovo, Imperial Script, BeauRivage
```

## Comportamento (replicado 1:1 do original)
1. Capa fullscreen com monograma A&R + selo de cera (borda iluminada pulsando).
2. Toque → selo "abre" + capa fade out 1.4s + vídeo fade in 0.8s + música simultânea.
3. Vídeo sai 0.8s antes do fim (fade 1.4s) → botão flutuante play/pause aparece.
4. Seções: hero (nomes, data, local, foto) → countdown → cerimônia/local + mapa →
   RSVP (form → WhatsApp) → final.
5. Countdown real até 27/09/2026 14:00 (fuso -03:00).

Detalhes da investigação: `01-ANATOMIA-TRANSICAO.md`.

## Para substituir mídias (cliente final)
- **Vídeo do casal**: trocar `assets/video-abertura.mp4` (ideal 720x1280, 4-6s).
- **Música**: trocar `assets/musica.mp3`.
- **Foto do hero**: trocar `assets/casal.webp`.
- **Capa (arte)**: gerar com o prompt de `02-PROMPT-CAPA.md`, salvar `assets/capa.png`
  e usar no `#weiOverlay` (instrução no doc 01).

## Abrir
Duplo clique em `index.html` (funciona offline — fontes/mídias locais).
