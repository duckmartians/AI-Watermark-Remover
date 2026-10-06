<h1 align="center">AI Watermark Remover</h1>

<p align="center"><b>Pinte sobre um logo, assinatura, texto sobreposto ou marca d'água em uma imagem ou vídeo - a IA preenche a área de forma natural, direto no seu computador, sem internet.</b></p>

<p align="center">
  <a href="README.md">English</a> ·
  <a href="README.vi.md">Tiếng Việt</a> ·
  <a href="README.bn.md">বাংলা</a> ·
  <a href="README.hi.md">हिन्दी</a> ·
  <b>Português (BR)</b> ·
  <a href="README.ru.md">Русский</a> ·
  <a href="README.tr.md">Türkçe</a> ·
  <a href="README.ur.md">اردو</a> ·
  <a href="README.zh_CN.md">简体中文</a>
</p>

<p align="center">
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="Baixar Lite para Windows" src="https://img.shields.io/badge/Baixar-Windows%20Lite-0078D6?style=for-the-badge&logo=windows&logoColor=white"></a>&nbsp;
  <a href="https://github.com/duckmartians/AI-Watermark-Remover/releases/latest"><img alt="Baixar Lite para macOS (Apple Silicon)" src="https://img.shields.io/badge/Baixar-macOS%20Apple%20Silicon%20Lite-000000?style=for-the-badge&logo=apple&logoColor=white"></a>&nbsp;
  <a href="https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3"><img alt="Baixar Pro para Windows (Google Drive)" src="https://img.shields.io/badge/Baixar-Windows%20Pro-76B900?style=for-the-badge&logo=windows&logoColor=white"></a>
</p>

---

## Instalação

### Passo 1 - Escolha a edição certa para o seu computador

Há duas edições. A **Lite** remove marcas d'água de **imagens** e roda na CPU. A **Pro** processa **imagens e vídeos** e precisa de um PC Windows com placa NVIDIA. O título da janela mostra **"Lite"** ou **"Pro"**, para você saber qual está usando.

| Seu computador | Download | Google Drive | Observações |
|---|---|---|---|
| 🪟 **Windows 10/11 (64 bits)** - Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`Windows_AI_Watermark_Remover_Lite_…zip`) | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Só imagens · não precisa de placa de vídeo |
| 🍎 **Mac com chip Apple (M1/M2/M3/M4)** - Lite | [Releases](https://github.com/duckmartians/AI-Watermark-Remover/releases/latest) (`MacOS_AI-Watermark-Remover-Lite-arm64_…dmg`) | [macOS](https://drive.google.com/drive/u/0/folders/1xKEA4WndYDrLD1c95MQRX2KhTVB_Op8l) | Só imagens · não há versão para Mac Intel |
| 🪟 **Windows 10/11 (64 bits) + GPU NVIDIA** - Pro | - | [Windows](https://drive.google.com/drive/u/0/folders/1FwJ8C8Rx-nqpOh5wErXWz-p3LucWNwW3) | Imagens **e vídeo** · a edição Pro é publicada só no Google Drive |

> A Pro precisa de uma placa **NVIDIA** com CUDA - placas AMD e Intel não são suportadas. Se você não tem uma, use a Lite (só imagens).

**Requisitos do sistema**

| | |
|---|---|
| **Lite (imagens)** | Windows 10/11 64 bits ou macOS com Apple Silicon · sem GPU · 4 GB+ de RAM |
| **Pro (imagens + vídeo)** | Só Windows 10/11 64 bits · GPU NVIDIA com CUDA, mínimo 4 GB de VRAM (6-8 GB recomendados para HD / clipes longos) · 8 GB+ de RAM |
| **CPU** | 64 bits com suporte a AVX2 |
| **Pré-requisitos (Windows)** | Visual C++ Redistributable 2015-2022 x64; a Pro também precisa de um driver NVIDIA atualizado |

### Passo 2 - Instalar

<details open>
<summary><b>🪟 No Windows</b></summary>

1. **Lite:** baixe o `.zip` em Releases e **extraia**. **Pro:** baixe da pasta do Google Drive.
2. Execute o instalador baixado (ou, se for uma pasta pronta para uso, abra **`AI Watermark Remover Lite.exe`** / **`AI Watermark Remover Pro.exe`** dentro dela).
3. Se aparecer **"Windows protected your PC"** (SmartScreen): clique em **More info** → **Run anyway**. *(O app não é assinado com um certificado pago, por isso é sinalizado - não é vírus.)*
4. O instalador pede permissão de administrador (instala em Program Files) e pode criar um atalho na Área de Trabalho. Abra o app pelo **Menu Iniciar** ou pela **Área de Trabalho**.

Lite e Pro são instalações separadas - você pode ter as duas no mesmo PC e desinstalar cada uma independentemente.

</details>

<details open>
<summary><b>🍎 No macOS</b></summary>

1. Abra o **`.dmg`** baixado e **arraste o AI Watermark Remover Lite para a pasta Aplicativos**.
2. Vá em **Aplicativos**, clique com o **botão direito** (ou Control-clique) em **AI Watermark Remover Lite** → **Abrir** → clique em **Abrir** de novo na caixa de diálogo. *(O app não é assinado pela Apple, então na **primeira vez** é preciso abri-lo assim; depois abre normalmente.)*
3. Se o macOS disser que o app está **"danificado / não pode ser aberto"**, ou não houver botão Abrir, abra o **Terminal** e cole:
   ```bash
   xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"
   ```
   Depois abra o app novamente.

</details>

A primeira abertura pode demorar um pouco mais; as seguintes são mais rápidas.

### Passo 3 - Grátis, sem conta

As duas edições são **gratuitas** - sem conta, sem chave de licença, sem limite de arquivos. Os modelos de IA vêm dentro do app, então ele não baixa nada enquanto roda e **nunca envia suas imagens ou vídeos** para lugar nenhum; tudo funciona offline.

---

## Primeira execução

1. **Abra um arquivo.** Clique no botão **📄** para escolher um ou mais arquivos, no **📁** para abrir uma pasta inteira, ou **arraste e solte** arquivos na janela. Se os arquivos tiverem proporções diferentes, o app pergunta qual proporção carregar (ou todas).
2. **Pinte sobre a marca d'água.** Escolha **Pincel**, **Caixa** ou **Texto** na coluna de ferramentas; a área pintada aparece em **vermelho suave**. Cubra tudo e passe um pouco das bordas - fica melhor do que pintar de menos.
3. **Clique em Executar.** O resultado substitui a área pintada. Com vários arquivos abertos, **Executar tudo** aplica a mesma área pintada a todos os arquivos do mesmo tamanho.
4. **Clique em Salvar** e escolha uma pasta de saída (o app pergunta toda vez). Ative **Adicionar _clean** antes se quiser manter os originais.

---

## Recursos

- **Pinte, desenhe uma caixa ou digite** - pinte livremente com o Pincel, arraste uma Caixa para cobrir rápido, apague o excesso com Apagar, ou digite um texto sobre uma marca d'água de texto para cobri-la com precisão. O texto é só um marcador - some depois do processamento e nunca fica gravado na imagem.
- **Corrija a seleção** - Desfazer / Refazer, Limpar toda a área pintada, ou Original para restaurar a imagem.
- **Processamento em lote** - **Executar tudo** aplica a área pintada atual a todos os arquivos abertos com a mesma proporção; arquivos com outra proporção são ignorados e contados no final.
- **Remoção de marca d'água em vídeo (Pro)** - a IA processa o vídeo quadro a quadro, trabalha só na área em volta da marca d'água, devolve o resultado ao quadro original e mantém o áudio original. Um player embutido permite percorrer o clipe com qualidade de prévia de 100 / 75 / 50 / 25%.
- **Salvar sem sobrescrever** - Salve um arquivo e vá para o próximo, ou **Salvar tudo** os arquivos processados em uma pasta; **Adicionar _clean** coloca um sufixo nos novos arquivos (`foto.png` → `foto_clean.png`).
- **Offline e privado** - tudo roda no seu computador; nada é enviado.
- **9 idiomas de interface** - English, Tiếng Việt, বাংলা, हिन्दी, Português (BR), Русский, Türkçe, اردو, 简体中文 - troque pelo ícone do globo.

---

## Ferramentas e controles

### 📂 Abrir

**📄** abre um ou mais arquivos, **📁** abre uma pasta inteira, ou arraste arquivos direto para a janela. Com vários arquivos aparece uma faixa de miniaturas embaixo - clique numa miniatura para trocar, ou no **×** para tirá-la da lista. A Lite só aceita imagens; arquivos de vídeo são filtrados.

### 🖌 Ferramentas

| Ferramenta | Use para |
|---|---|
| **Pincel** | Pintar sobre a marca d'água (segure o botão esquerdo e arraste). Ajuste o tamanho no controle deslizante, com `Ctrl` + roda do mouse, ou `[` / `]`. Segure o **botão direito** para apagar enquanto pinta. |
| **Caixa** | Arrastar um retângulo sobre a marca d'água para cobrir rápido. |
| **Apagar** | Remover o excesso de pintura. |
| **Texto** | Digitar texto sobre uma marca d'água de texto para cobri-la com precisão (só imagens). `Delete` remove o texto selecionado. |

Clique de novo no botão da ferramenta, ou pressione **Esc**, para desmarcá-la. **Desfazer / Refazer / Limpar / Original** ficam na mesma coluna.

### ▶ Executar

**Executar** processa o arquivo que você está vendo; **Executar tudo** (aparece com 2+ arquivos abertos) processa todos os arquivos com a mesma proporção. Durante o processamento, os botões viram **Parar** / **Parar tudo**. Os resultados ficam no app até você salvá-los.

### 🎬 Vídeo (Pro)

Abra um vídeo, pause em qualquer quadro e pinte sobre a marca d'água com Pincel ou Caixa (começar a pintar pausa a reprodução). Use o botão de play e a barra de busca para conferir o clipe, e o menu de qualidade (100 / 75 / 50 / 25%) para deixar a prévia leve. O vídeo é processado quadro a quadro, então é **bem mais lento que imagens** - deixe rodar. Quando terminar, salve com **Salvar** ou **Salvar tudo** como uma imagem; a saída é um `.mp4`.

### 💾 Salvar

**Salvar** grava o resultado atual e passa para o próximo arquivo; **Salvar tudo** grava todos os arquivos processados em uma pasta. O app pergunta a pasta de saída toda vez. Marque **Adicionar _clean** para acrescentar `_clean` ao nome em vez de reutilizar o nome original.

### 🔍 Visualização

Roda do mouse para zoom, segure o botão do meio e arraste para mover, **F** ou clique duplo para ajustar à janela. O ícone de **casa** abre a página inicial; o **globo** troca o idioma.

### ⌨️ Atalhos de teclado

| Ação | Tecla |
|---|---|
| Desfazer / Refazer | `Ctrl+Z` / `Ctrl+Shift+Z` |
| Tamanho do pincel | `Ctrl` + roda do mouse, ou `[` / `]` |
| Ajustar à janela | `F`, `0` ou clique duplo |
| Desmarcar ferramenta | `Esc` |
| Apagar rápido (usando o Pincel) | Segure o **botão direito** |
| Mover a imagem | Segure o **botão do meio** e arraste |

### 🗂 Formatos suportados

- **Imagens:** PNG, JPG/JPEG, WEBP, BMP, TIFF, PPM/PGM/PBM/PNM.
- **Vídeo (Pro):** MP4, M4V, MOV, WEBM, MKV, AVI, FLV, WMV, MPG/MPEG, TS/M2TS/MTS, 3GP, OGV. A saída é salva como `.mp4`.

---

## Onde ficam seus dados

| O quê | Windows | macOS |
|---|---|---|
| Imagens / vídeos de saída | A pasta que você escolhe ao salvar | A pasta que você escolhe ao salvar |
| Configurações (idioma, Adicionar _clean) | Registro: `HKEY_CURRENT_USER\Software\Duckmartians\AI Watermark Remover` | `~/Library/Preferences/com.duckmartians.AI Watermark Remover.plist` |
| Resultados não salvos (temporários) | `%TEMP%\AIWatermarkRemover_work` | `AIWatermarkRemover_work` na pasta temporária do sistema |
| Log de falhas | `%APPDATA%\AI Watermark Remover\crash.log` | `~/AI Watermark Remover/crash.log` |

A pasta temporária é limpa sempre que o app abre - **salve seus resultados antes de fechar o app**.

---

## Solução de problemas

**O Windows bloqueia com "Windows protected your PC"** - clique em **More info → Run anyway**. O app não é assinado com um certificado pago, por isso é sinalizado - não é vírus.

**O macOS diz que o app está danificado / não pode ser aberto** - ele não é assinado pela Apple. Na primeira vez, botão direito → **Abrir**, ou rode `xattr -dr com.apple.quarantine "/Applications/AI Watermark Remover Lite.app"`.

**Não consigo abrir vídeos** - você está na edição **Lite**, que só processa imagens. Instale a **Pro** (Windows + placa NVIDIA) para remover marcas d'água de vídeos.

**Ao salvar, aparece que vídeos são exportados com "Executar"** - esse vídeo ainda não foi processado. Clique em **Executar** (ou **Executar tudo**) primeiro e depois em **Salvar**.

**Executar tudo ignorou alguns arquivos** - Executar tudo só processa arquivos com a mesma proporção do arquivo em que você pintou. Abra os outros separadamente, ou escolha a proporção deles ao abrir.

**Ficam marcas leves depois da remoção** - pinte de forma mais completa e um pouco além das bordas da marca d'água, e Execute de novo. Áreas grandes sobre fundos detalhados ainda podem deixar vestígios.

**O vídeo está muito lento** - é normal: a IA processa cada quadro, então vídeo demora bem mais que imagem. Deixe rodar; clipes mais curtos e uma placa com mais VRAM terminam mais rápido.

**O app fecha sozinho** - envie o arquivo `crash.log` (veja a tabela acima) ao relatar o problema.

---

Remova marcas d'água e logos apenas de imagens e vídeos que são seus ou que você tem direito de editar.
