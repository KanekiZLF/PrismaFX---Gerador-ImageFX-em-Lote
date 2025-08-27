# PrismaFX

[![Tutorial em Vídeo](https://img.shields.io/badge/Tutorial-YouTube-red)](https://www.youtube.com/watch?v=f_NrxFAwhZ0)
[![Licença](https://img.shields.io/badge/Licença-MIT-blue.svg)](https://github.com/KanekiZLF/PrismaFX---Gerador-ImageFX-em-Lote/blob/master/license.txt)

PrismaFX é uma ferramenta de automação para Windows que potencializa a sua criatividade, permitindo a geração de imagens em lote através da tecnologia ImageFX do Google Labs.

---

## 🖼️ Visão Geral

![Screenshot do PrismaFX](https://img001.prntscr.com/file/img001/QWSIDYRWQk-r5AyoV_ttMw.png)

## ✨ Funcionalidades

- **Geração em Lote:** Crie ou carregue de 1 a 50 prompts e gere todas as imagens de uma só vez.
- **Carregador de Arquivos:** Importe listas de prompts diretamente de um arquivo `.txt` para automação rápida.
- **Controle Total:** Ajuste a proporção (quadrado, retrato, paisagem) e o número de imagens por prompt.
- **Consistência com Seed:** Trave uma "semente" (seed) para gerar imagens com um estilo visual consistente.
- **Visualizador Integrado:** Navegue pelos resultados de cada prompt diretamente na interface do programa.
- **Verificador de Atualizações:** Seja notificado sobre novas versões diretamente pelo menu de configurações.
- **Interface Moderna:** Tema claro e escuro para se adaptar à sua preferência.

## 🚀 Começando a Usar

Nenhuma instalação é necessária! O programa é um executável portátil.

1.  Baixe o arquivo `PrismaFX.exe` da versão mais recente.
2.  Execute o arquivo e comece a criar!

## 📖 Como Usar

O uso do PrismaFX é dividido em 5 passos simples:

#### 1. Obter o Token de Autenticação

O programa precisa de um token de acesso para se comunicar com a API do ImageFX. Para obtê-lo:

1.  **Acesse o site:** Abra o [ImageFX do Google Labs](https://labs.google/fx/pt/tools/image-fx) no seu navegador.
2.  **Abra o Console:** Pressione a tecla `F12` para abrir as "Ferramentas de Desenvolvedor".
3.  **Vá para a aba "Console"**.
4.  **Copie o código abaixo** e cole-o no console:
    ```javascript
    let script = document.querySelector("#__NEXT_DATA__");
    let obj = JSON.parse(script.textContent);
    console.log(obj.props.pageProps.session.access_token);
    ```
5.  **Pressione Enter.** O seu token de acesso pessoal será exibido no console.
6.  **Copie o token** e cole-o no campo "Token de Autenticação" do PrismaFX.

> ✨ **Dica:** Dentro do programa, o botão **`?`** abre uma janela de ajuda com este guia e um botão para copiar o código automaticamente. Você também pode assistir ao **[tutorial em vídeo](https://www.youtube.com/watch?v=f_NrxFAwhZ0)**.

#### 2. Configurar os Prompts

Você pode preparar vários prompts para serem executados em sequência de duas maneiras:

**Opção A: Carregar de um Arquivo (Recomendado para Lotes Grandes)**

1.  Crie um arquivo de texto (`.txt`) com seus prompts. O formato deve seguir este padrão:
    ```txt
    Prompt 1 – A despedida na Antártida

    Um pinguim cartoon 3D estilo Disney/Pixar chamado Picolino, corpo rechonchudo, penas pretas e brancas brilhantes, olhos grandes expressivos, bochechas fofas, usando uma mochila amarela e carregando um caderninho de anotações preso com elástico. Ele está em pé sobre uma rocha de gelo, olhando o horizonte cheio de icebergs iluminados por um pôr do sol rosado e laranja. Atmosfera mágica, cinematográfica, leve névoa no ar, reflexo dourado no mar congelado. Ângulo: plano médio com leve contra-plongée para transmitir coragem.
    
    Prompt 2 – Escondido no navio
    
    Picolino, o pinguim cartoon 3D estilo Disney/Pixar, dentro do porão de um navio de carga, escondido em uma caixa de madeira aberta, com apenas seus olhos grandes e curiosos espiando pela fresta. Sua mochila amarela aparece levemente, e o caderninho está sobre suas patas. Ambiente escuro iluminado por uma única lâmpada pendurada, criando um contraste engraçado e dramático. Estilo vibrante, texturas detalhadas de madeira e metal enferrujado. Ângulo: close divertido, destacando sua expressão curiosa.
    
    Prompt 3 – Chegada à cidade
    
    Picolino, pinguim cartoon 3D Disney/Pixar, saindo de dentro de uma caixa no porto movimentado de uma...
    ```
2.  No PrismaFX, ao lado do seletor de "Quantidade de Prompts", clique no botão **"Carregar de TXT..."**.
3.  Selecione seu arquivo. O programa irá ler, formatar e carregar todos os prompts automaticamente.

**Opção B: Configuração Manual**

- **Quantidade de Prompts:** Selecione o número total de prompts que você deseja usar.
- **Navegação:** Use os botões **`< Anterior`** e **`Próximo >`** para navegar entre os campos de prompt.
- Escreva ou edite a descrição detalhada em cada campo.

#### 3. Ajustar as Opções

Personalize os parâmetros de geração para cada lote:

- **Proporção:** Escolha entre Quadrado (1:1), Retrato (9:16) ou Paisagem (16:9).
- **Imagens por Prompt:** Defina quantas imagens (de 1 a 4) devem ser geradas para cada prompt.
- **Seed:** Digite um número de "semente" para obter resultados mais consistentes ou deixe em branco para gerar uma seed aleatória. Marque a caixa **"Travar Seed"** se quiser usar o mesmo número para todos os prompts do lote.

#### 4. Gerar as Imagens

Quando tudo estiver pronto, clique no botão principal:

- **Gerar Todas as Imagens**: O PrismaFX começará a processar cada prompt, um por um. Acompanhe o progresso pela barra de status. Se precisar parar, clique no botão **"Cancelar"**.

#### 5. Visualizar e Salvar

As imagens geradas aparecerão no painel da direita.

- Use os botões **`< Anterior`** e **`Próximo >`** abaixo do painel de imagens para navegar entre os resultados de cada prompt.
- Clique em **"Regerar Atual"** para tentar um novo resultado para o prompt que está sendo exibido.
- Clique em **"Salvar Página..."** para abrir uma janela e escolher uma pasta no seu computador para salvar as imagens do prompt atual.

## 🛠️ Desenvolvido Com

Este projeto foi construído utilizando as seguintes tecnologias:

* **Linguagem:** Python
* **Interface Gráfica:** CustomTkinter
* **Requisições de Rede:** Requests
* **Manipulação de Imagens:** Pillow
* **Empacotamento:** PyInstaller

---

## ⚠️ Aviso Importante

Este programa utiliza uma API **não oficial** para se comunicar com os serviços do Google ImageFX e não possui afiliação, patrocínio ou endosso do Google. Por depender de um serviço não documentado, a ferramenta pode parar de funcionar a qualquer momento se houverem alterações na plataforma original. Use por sua conta e risco.

## 📜 Licença

Este projeto é distribuído sob a Licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

### 📩 Quer o Código Fonte? 
<p align="center">
  Interessado no código fonte? Me mande um email: kanekizlf4@gmail.com
</p>

---
<p align="center">
  Desenvolvido por Luiz F. R. Pimentel
</p>
