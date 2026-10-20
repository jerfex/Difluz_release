# ✨ Difluz

*Luz sobre as suas alterações* — **Difluz** = *diff* + *luz*.

---

## 💡 O que é o Difluz?

O **Difluz** é uma aplicação desktop **100% local e offline** criada para você **revisar as alterações do seu repositório Git antes de compartilhá-las** (antes de fazer commit, push ou abrir um Pull Request).

Com o uso cada vez maior de assistentes de Inteligência Artificial no dia a dia de programação, geramos muito código rapidamente. O Difluz coloca uma etapa visual, organizada e segura para você conferir arquivo por arquivo tudo o que mudou na sua máquina antes de enviar para o repositório da equipe.

- 🔒 **Privacidade Total:** Funciona totalmente offline. Nenhum código ou informação do seu projeto sai do seu computador.
- 🛡️ **Seguro por Padrão:** Você tem controle total sobre o seu repositório, sem risco de comandos destrutivos automáticos.

---

## 📥 Download e Instalação (Linux x64)

### Pré-requisito
- Ter o **Git** instalado no sistema (`git --version` no terminal).

### Opção 1 — Instalar direto pelo terminal (Ubuntu, Debian, Linux Mint, Pop!_OS, Zorin OS e derivados)

Copie e cole o comando abaixo no terminal para baixar e instalar automaticamente:

```bash
wget -O difluz_1.2.0_amd64.deb https://github.com/jerfex/Difluz_release/raw/main/releases/difluz_1.2.0_amd64.deb && sudo apt install ./difluz_1.2.0_amd64.deb
```

### Opção 2 — Download manual do instalador `.deb`

1. Clique no link abaixo para baixar o arquivo de instalação:
   - 👉 [**Baixar `difluz_1.2.0_amd64.deb`**](https://github.com/jerfex/Difluz_release/raw/main/releases/difluz_1.2.0_amd64.deb)
2. Na pasta onde baixou o arquivo, instale pelo terminal:
   ```bash
   sudo apt install ./difluz_1.2.0_amd64.deb
   ```
   *(Ou dê dois cliques no arquivo `.deb` para instalar pelo gerenciador de pacotes gráfico do sistema).*
3. Abra o **Difluz** pelo menu de aplicativos do seu sistema ou digitando `difluz` no terminal.

---

## 📘 Tutorial: Como Usar o Difluz

### 1. Abrir seu projeto
- Clique em **Abrir repositório…** e selecione a pasta do seu projeto Git (ou escolha um projeto na lista de **Recentes**).
- Na barra lateral esquerda, você verá a *branch* atual, o resumo de todos os arquivos alterados (modificados, adicionados, excluídos, não rastreados ou em conflito) e o total de linhas adicionadas (`+`) e removidas (`−`).

### 2. Analisar as alterações (Diff)
- Clique em qualquer arquivo da lista (ou navegue rapidamente com `Alt + ↓` e `Alt + ↑`).
- Escolha entre a visualização **Lado a Lado** (comparando o antes e o depois) ou **Unificada**.
- Alterne entre mudanças *Staged* e *Não Staged* e expanda as linhas de contexto sempre que precisar ver mais trechos do arquivo.

### 3. Conferir os Alertas de Atenção
- O Difluz sinaliza automaticamente pontos que merecem cuidado extra antes de subir o código:
  - Arquivos sensíveis (como `.env` e configurações locais).
  - Possíveis chaves, senhas ou tokens esquecidos no código (exibidos de forma mascarada).
  - Arquivos binários ou muito grandes.
  - Mudanças em dependências ou pipelines de CI/CD.

### 4. Marcar arquivos como revisados e criar anotações
- Terminou de conferir um arquivo? Clique em **Marcar como revisado** (ou pressione `Alt + R`).
- **Controle inteligente:** Se você editar novamente na sua IDE um arquivo que já tinha sido marcado como revisado, o Difluz detecta a mudança automaticamente e avisa que ele foi **alterado após a revisão**.
- Use o painel inferior para adicionar **Observações** no arquivo (ou em linhas específicas) caso queira lembrar de algum ajuste antes do commit.

### 5. Concluir a revisão
- Quando revisar todos os arquivos desejados, clique em **Concluí a revisão**.
- O aplicativo registra que aquele estado exato do projeto foi revisado. Se novas alterações forem feitas depois, o status muda para **Revisão desatualizada**, mantendo o seu histórico organizado.

### 6. Fluxo Git e Gerador de `.gitignore` integrados
- **Painel Git (`Git…` na barra lateral):** Permite fazer *stage/unstage*, *commit*, criar ou trocar de *branch*, realizar *merge*, gerenciar *stash* e fazer *fetch*, *pull* e *push* sem precisar sair do aplicativo.
- **Gerador de `.gitignore` (`.gitignore…` na barra lateral):** Identifica o tipo de tecnologia do seu projeto e sugere automaticamente as regras que faltam no seu `.gitignore`, mostrando uma prévia antes de salvar.
- **Configurações:** Escolha entre tema Claro, Escuro ou do Sistema, ajuste a densidade visual e selecione o idioma (**Português (Brasil)**, **Português (Portugal)** ou **Inglês**).

---

## ⌨️ Atalhos Rápidos

| Atalho | Ação |
| :--- | :--- |
| `F5` | Atualizar estado do repositório |
| `Alt + ↓` / `Alt + ↑` | Próximo arquivo / Arquivo anterior |
| `F8` / `Shift + F8` | Próximo bloco / Bloco anterior de alteração |
| `Alt + R` | Marcar ou desmarcar arquivo como revisado |
| `Ctrl + F` | Buscar arquivo na lista |

---

## 🗺️ Próximas Versões e Outros Sistemas Operacionais

Atualmente, esta release está disponível para **Linux (x64)**.

Novas versões com melhorias contínuas e instaladores oficiais para outros sistemas operacionais serão liberadas em breve neste mesmo repositório:
- 🐧 **Linux (`.deb` x64):** ✅ Disponível (v1.2.0)
- 🪟 **Windows (10/11):** 🔜 Em breve
- 🍎 **macOS:** 🔜 Em breve

Acompanhe este repositório para baixar as próximas atualizações!

---

## 💬 Feedback e Sugestões

Encontrou algum problema durante o uso ou tem ideias para as próximas versões?
Abra uma [**Issue**](https://github.com/jerfex/Difluz_release/issues) aqui no repositório!
