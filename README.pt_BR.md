# AI Watermark Remover — Guia do Usuário

<p align="left">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest">
    <img src="https://img.shields.io/badge/Windows-%F0%9F%92%BB-0078D6?style=for-the-badge&logo=windows&logoColor=white">
  </a>
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest">
    <img src="https://img.shields.io/badge/macOS-%F0%9F%8D%8E-000000?style=for-the-badge&logo=apple&logoColor=white">
  </a>
</p>
<p align="left">
  <a href="https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3">
    <img src="https://img.shields.io/badge/Windows-Drive%20backup-4285F4?style=flat-square&logo=googledrive&logoColor=white">
  </a>
  <a href="https://drive.google.com/drive/u/0/folders/1xKEA4WndYDrLD1c95MQRX2KhTVB_Op8l">
    <img src="https://img.shields.io/badge/macOS-Drive%20backup-4285F4?style=flat-square&logo=googledrive&logoColor=white">
  </a>
</p>
<p align="left">
  <a href="https://duckmartians.info">
    <img src="https://img.shields.io/badge/Homepage-Visit-0A66C2?style=flat-square&logo=google-chrome&logoColor=white">
  </a>
  <a href="https://discord.gg/munMZEBMw5">
    <img src="https://img.shields.io/badge/dynamic/json?url=https://discord.com/api/guilds/1369302820037201981/widget.json&query=$.presence_count&label=Discord&color=5865F2&logo=discord&style=flat-square">
  </a>
</p>

🌐 [English](README.md) · [Tiếng Việt](README.vi.md) · [বাংলা](README.bn.md) · [हिन्दी](README.hi.md) · **Português (BR)** · [Русский](README.ru.md) · [Türkçe](README.tr.md) · [اردو](README.ur.md) · [简体中文](README.zh_CN.md)

Este aplicativo ajuda você a **remover logotipos, marcas d'água, assinaturas e textos sobrepostos de imagens e vídeos**.
Basta **pintar sobre o que você quer eliminar** e o aplicativo preenche a área de forma natural. Tudo funciona
**no seu próprio computador** — **sem precisar de internet**, e suas imagens/vídeos **nunca são enviados para lugar nenhum**.

---
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/dbcb0fad-cc38-49d6-b9c6-acd1c0e16983" />
<img width="804" height="852" alt="image" src="https://github.com/user-attachments/assets/f07d1f33-e835-4c6c-b5b6-6b8db94b9cb9" />

## Instalar e abrir

1. Execute o instalador (ou descompacte a pasta, se você recebeu um arquivo compactado).
2. Abra o **AI Watermark Remover** (pela Área de Trabalho, pelo menu Iniciar ou pelo arquivo `.exe`).

> **O Windows mostra "Windows protected your PC" (O Windows protegeu seu PC)?**
> Este é o aviso padrão para aplicativos sem um certificado de assinatura pago — **não é um vírus**.
> Clique em **More info → Run anyway** (Mais informações → Executar mesmo assim) para abri-lo.

A primeira inicialização pode demorar um pouco mais; as próximas são mais rápidas.

**Existem duas edições:** a edição **Pro** (imagens + vídeo) e a edição **Lite** (somente imagens, mais leve).
Verifique o título da janela para diferenciá-las: **"Pro"** = edição completa, **"Lite"** = edição leve (não abre vídeos).

---

## Requisitos do sistema

| | **Lite** (imagens) | **Pro** (imagens + vídeo) |
|---|---|---|
| Plataforma | **Windows 10/11** 64 bits **e macOS** | **somente Windows 10/11 64 bits** — *sem macOS* |
| CPU | 64 bits com **AVX2** | 64 bits com **AVX2** |
| GPU | **não é necessária** — roda na CPU | **GPU NVIDIA com CUDA obrigatória** |
| VRAM | — | 4 GB no mínimo · **6–8 GB recomendados** (HD / clipes longos) |
| RAM | 4 GB+ | 8 GB+ |
| Instale também (Windows) | **Visual C++ Redistributable 2015–2022 x64** | o mesmo + um **driver NVIDIA** atualizado |

- A edição **Pro** roda sua IA de vídeo nos **núcleos CUDA da NVIDIA**, por isso ela é **exclusiva do Windows e exige uma placa de vídeo NVIDIA** — aproximadamente uma **RTX 2060 (RTX 20-series / GTX 16-series, "Turing") ou mais recente**.
- **O macOS não tem CUDA** → em um Mac, use a edição **Lite** (imagens). GPUs AMD/Intel também **não são compatíveis** com o motor de vídeo do Pro.
- A remoção em **imagens** funciona bem **na CPU** em **ambas** as edições — nenhuma placa de vídeo é necessária.

---

## Como usar — 4 passos

### Passo 1 — Abra uma imagem/vídeo
- Clique no botão de **documento** para escolher um ou mais arquivos, ou no botão de **pasta** para abrir uma pasta inteira.
- Ou **arraste e solte** imagens/vídeos diretamente na janela.
- Com vários arquivos, você verá uma faixa de miniaturas na parte inferior; cada item tem um **×** para removê-lo da lista.

### Passo 2 — Pinte sobre o que remover
Escolha uma ferramenta na coluna da esquerda e pinte/contorne a marca d'água (a área pintada aparece em **vermelho suave**):

| Ferramenta | Use para |
|----|---|
| **Pincel** | Pintar sobre a marca d'água (segure o botão esquerdo do mouse e arraste). Ajuste o tamanho do pincel com o controle deslizante abaixo. |
| **Caixa** | Arrastar um retângulo sobre a marca d'água para cobri-la rapidamente. |
| **Borracha** | Apagar o excesso de pintura. |
| **Texto** | Digitar um texto para cobrir com precisão uma marca d'água em formato de texto. Este texto é apenas um **marcador** — ele desaparece após o processamento e não fica gravado na imagem. |

Pintou demais? Use **Desfazer / Refazer / Limpar tudo / Redefinir** na coluna da esquerda.
Clique novamente no botão da ferramenta (ou pressione **Esc**) para desativá-la.

> **Dica:** cubra a marca d'água por completo e ultrapasse um pouco as bordas — os resultados ficam melhores do que pintando de menos.

### Passo 3 — Clique em Executar
- **Executar** — processa a imagem/vídeo aberto no momento.
- **Executar tudo** — processa em lote todos os arquivos **com o mesmo tamanho de quadro** na lista
  (disponível apenas quando há 2 ou mais arquivos).

### Passo 4 — Salvar
- Clique em **Salvar**. **A cada vez que você salva, o aplicativo pede para você escolher uma pasta** para os arquivos de saída.
- Quer manter os originais? Ative a opção **"Adicionar _clean"** — os novos arquivos recebem o sufixo `_clean`
  no nome (por exemplo, `photo.png` → `photo_clean.png`), para que o original não seja sobrescrito.

---

## Processamento de vídeo (edição Pro)

- Os vídeos **não são salvos com o botão Salvar**. Clique em **Executar** (um vídeo) ou **Executar tudo**
  (vários vídeos); o aplicativo pede uma pasta de salvamento quando começa.
- O vídeo é processado quadro a quadro com IA, por isso é **muito mais lento do que imagens** — apenas deixe rodando.

### Controles deslizantes de velocidade ⇄ qualidade

Abaixo do controle deslizante **Tamanho do pincel** (coluna da esquerda, apenas **Pro**) há quatro controles deslizantes para trocar velocidade por qualidade. Passe o mouse sobre qualquer controle para ver uma dica; suas configurações são lembradas.

| Controle | O que controla | Mais rápido | Mais nítido |
|---|---|---|---|
| **Resolution** | Resolução de processamento — a maior alavanca de velocidade. Menor = muito mais rápido, área apagada um pouco suave. | ~**50** | **100** |
| **Motion** | O quão minuciosamente o movimento entre quadros é analisado (a qualidade quase não muda). | **2–4** | 20 |
| **Frames** | Quantos quadros próximos são tratados juntos. | menor | maior |
| **Reference** | Espaçamento ao escolher os quadros de referência. | **maior** | menor |

- Quer que fique rápido? Defina **Resolution ≈ 50** e **Motion ≈ 4** (os padrões já favorecem a velocidade).
- A área apagada parece borrada? Aumente **Resolution** em direção a **100**.
- Isso afeta apenas o **vídeo**; as imagens não são afetadas.

---

## Visualização e utilidades

- **Roda do mouse**: aproximar / afastar · **Segure o botão do meio e arraste**: mover · **F** ou **clique duplo**: ajustar à janela.
- Ícone de **casa**: abre a página inicial. Ícone de **globo**: muda o idioma (9 idiomas disponíveis, incluindo vietnamita).

## Atalhos de teclado

| Ação | Tecla |
|---|---|
| Desfazer / Refazer | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Mudar o tamanho do pincel | `Ctrl` + roda do mouse |
| Ajustar à janela | `F` ou clique duplo |
| Desativar ferramenta | `Esc` |
| Apagar rápido (usando o Pincel) | Segure o **botão direito do mouse** |

---

## Formatos suportados

- **Imagens:** JPG, PNG, WEBP, BMP, TIFF e outros formatos de imagem comuns.
- **Vídeo:** MP4, MOV, MKV, AVI, WEBM, WMV, FLV… (edição Pro).

## Solução de problemas

| Sintoma | O que fazer |
|---|---|
| O Windows avisa ao abrir | Clique em **More info → Run anyway** (Mais informações → Executar mesmo assim) (o aplicativo é seguro, apenas não tem assinatura de código). |
| Não consigo abrir vídeos | Você está na edição **Lite** — somente imagens. Use a edição **Pro**. |
| Restam marcas fracas após a remoção | Pinte **de forma mais completa e ultrapassando um pouco as bordas**, depois execute novamente. |
| O vídeo está muito lento | Reduza o controle deslizante **Resolution** (≈50) e **Motion** (≈4) — veja a seção *Controles deslizantes de velocidade ⇄ qualidade*. Uma GPU NVIDIA com CUDA (RTX 2060+) é fortemente recomendada — veja *Requisitos do sistema*. |

Aproveite!
