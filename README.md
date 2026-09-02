# Drª Ester Barbosa — Landing Page

Landing page da **Drª Ester Barbosa**, cirurgiã-dentista (CRO-PE 21497), em Boa Viagem, Recife.

Site estático de arquivo único: HTML, CSS e JS em `index.html`, sem build, sem dependências
externas em tempo de execução. Basta servir a pasta.

```bash
python3 -m http.server 8000   # abre em http://localhost:8000
```

## Estrutura

```
index.html                 # a página inteira (marcação, estilos e scripts)
assets/
  css/fonts.css            # @font-face das fontes auto-hospedadas
  fonts/                   # Playfair Display + Poppins (woff2, subsets latin/latin-ext)
  img/                     # imagens otimizadas para a web
  originais/               # fotos originais, como recebidas (não usadas pela página)
```

### Imagens

| Arquivo | Uso |
| --- | --- |
| `logo-monograma.png` | monograma "B" branco (fundo escuro) — CTA final |
| `logo-monograma-escuro.png` | monograma "B" escuro (fundo claro) — header, favicon, mapa |
| `logo-completo.png` | logo com assinatura completa — rodapé |
| `ester-hero.jpg` | hero |
| `ester-jaleco.jpg` | seção "Sobre" |
| `ester-perfil.jpg` | seção "Propósito" |
| `ester-consultorio.jpg` | seção "Medo de dentista?" |
| `ester-celular.jpg`, `ester-janela.jpg`, `ester-notebook.jpg` | reserva |
| `caso-*.jpg` | galeria de antes e depois |
| `marca-paleta.jpg` | referência da paleta da marca |

Os PNGs de logo têm fundo transparente, gerados a partir da luminância dos originais.

## Identidade visual

Paleta monocromática, conforme o manual da marca (`assets/img/marca-paleta.jpg`):

| Cor | Hex |
| --- | --- |
| Pure White | `#FFFFFF` |
| Eerie Black | `#121212` |
| Dark Charcoal | `#2C2C2C` |

Tipografia: **Playfair Display** (títulos, serifada de alto contraste, ecoa o logo) e
**Poppins** (texto e interface, geométrica). Ambas auto-hospedadas — nenhuma requisição
a servidores de terceiros.

## Seções

Hero · credenciais · Sobre · Propósito · Tratamentos · Como funciona · Antes e depois ·
Depoimento do Dr. Flávio Venícius · Depoimentos de pacientes · Acolhimento ·
Formação · FAQ · Contato e horários · CTA final · Rodapé.

## Recursos

- Responsiva de 320 px a wide, sem rolagem horizontal
- Galeria com filtro por categoria e lightbox (setas e `Esc`)
- Carrossel de depoimentos, FAQ em acordeão, menu mobile
- Horário do dia atual destacado automaticamente
- Animações de entrada via `IntersectionObserver`, com `prefers-reduced-motion`
- SEO: meta tags, Open Graph e JSON-LD `Dentist` com `aggregateRating`

## Conteúdo a substituir

Os textos e números reais vieram do Google Meu Negócio e do Instagram da Drª Ester.
Foram redigidos para completar a página e devem ser revisados antes de publicar:

- **Tratamentos** — descrições dos 9 cards
- **Como funciona** — as 4 etapas da jornada do paciente
- **Acolhimento** — os 4 itens da seção "Medo de dentista?"
- **FAQ** — as 8 perguntas e respostas, em especial preços, pagamento e convênio
- **Legendas da galeria** — confirmar o procedimento de cada caso

Dados confirmados: telefone (81) 98491-8489, Instagram [@esterabarbosa](https://instagram.com/esterabarbosa),
CRO-PE 21497, endereço, horários e nota 5,0 com 39 avaliações no Google.

> As fotos de pacientes exigem autorização de uso de imagem antes da publicação.
