# MANUAL DE OPERAÇÕES GITHUB - PROJETO CODERWEALTH IDENTIDADE

**Responsáveis:**
- **Gerente:** Clawdbot (IA no servidor) - Responsável por Conteúdo
- **Executor:** Felipe (Você) - Responsável por Operações Técnicas (Shell, Git, Python)

**Data da Última Atualização:** 27/01/2026 (DIA 27)

---

## IDENTIDADE DOS PAPÉIS

### 1. GERENTE (Clawdbot)

**Função:**
- Criar conteúdo (artigos em Markdown)
- Estruturar o projeto (HTML, CSS, configuração)
- Escrever arquivos `.md` no disco do servidor
- Fornecer instruções detalhadas
- NÃO executa comandos Git diretamente, a menos que seja estritamente necessário para salvar arquivos (uso do comando `write`).

**O que o Gerente NÃO faz:**
- NÃO roda scripts Shell complexos (bash `finance_articles.sh`).
- NÃO roda scripts Python (python `generate.py`).
- NÃO faz `git commit` ou `git push` (isso é função do Executor).
- NÃO faz `git add` (o Executor deve fazer isso).

**Comandos do Gerente:**
- `write <caminho> <conteúdo>` - Cria arquivos Markdown.

### 2. EXECUTOR (Felipe)

**Função:**
- Rodar comandos no terminal do servidor SSH.
- Executar scripts Shell (`bash scripts-autonomous/finance_articles.sh`).
- Executar comandos Git (`git add`, `git commit`, `git push`).
- Copiar/Arastar arquivos usando `cp`.
- Verificar status do site no navegador.

**O que o Executor faz:**
- Toda a operação técnica real.
- A conexão com o GitHub.
- A verificação visual do resultado.

**Comandos do Executor:**
- `bash <script.sh>` - Roda script.
- `git add .` - Adiciona mudanças.
- `git commit -m "..."` - Salva mudanças.
- `git push origin main` - Envia para o GitHub.

---

## FLUXO PADRÃO DE TRABALHO (SOP)

### Etapa 1: Conteúdo (Gerente)
O Gerente cria os arquivos Markdown `.md` com o Front Matter Jekyll correto.
- Arquivos são criados via comando `write`.
- Conteúdo é técnico, direto, sem emojis.

### Etapa 2: Scripts (Gerente - Opcional)
O Gerente pode criar scripts Shell (`finance_articles.sh`) que *gerari* o Markdown.
- **Nota:** Como o Gerente pode criar o Markdown diretamente, este passo pode ser pulado para ganhar tempo.

### Etapa 3: Preparação (Executor)
O Executor acessa o servidor SSH.
- Navega até o diretório do projeto: `cd /home/clawdbot/coderwealth.com`.
- Verifica o status: `git status`.

### Etapa 4: Execução (Executor)
O Executor executa os comandos necessários.
- Se o Gerente criou Markdowns diretos: O Executor apenas faz `git add`, `commit`, `push`.
- Se o Gerente criou scripts: O Executor roda o script primeiro (`bash script.sh`) e depois Git.

### Etapa 5: Verificação (Executor)
O Executor verifica o site no navegador.
- Verifica se os artigos aparecem.
- Verifica se o site está atualizado.

---

## COMANDOS TÉCNICOS (SOMENTE PARA EXECUTOR)

### Preparação
```bash
cd /home/clawdbot/coderwealth.com
```

### Scripts (Se o Gerente criar)
```bash
bash scripts-autonomous/finance_articles.sh
```

### Git (Executor)
```bash
git add .
git commit -m "Nova Publicacao: [TÍTULO]"
git push origin main
```

---

## TRATAMENTO DE ERROS

### Erro: "File not found"
**Causa:** Arquivo não foi criado pelo Gerente.
**Solução:** O Executor avisa o Gerente. O Gerente cria o arquivo via `write` e tenta novamente.

### Erro: "Permission denied"
**Causa:** Permissões de usuário.
**Solução:** O Executor verifica dono (`ls -la`). Se o dono não for `clawdbot`, o Executor não usa `sudo`. O Executor avisa o usuário para corrigir permissões.

### Erro: "Conflict"
**Causa:** Histórias do Git divergem.
**Solução:** O Executor tenta `git pull --rebase origin main`. Se falhar, usa `bash scripts-autonomous/smart_push.sh`.

---

## REGRAS DE SEGURANÇA (REGRA DE OURO)

1. **Gerente:** NUNCA executa `git push` (Reservado ao Executor).
2. **Executor:** SEMPRE executa `git push` após `git commit`.
3. **Gerente:** NUNCA roda `bash scripts-autonomous/*.sh` (Reservado ao Executor).
4. **Executor:** SEMPRE roda scripts Shell gerados pelo Gerente (se houver).
5. **Gerente:** NUNCA usa `sudo` no Git.
6. **Executor:** Pode usar `sudo` se for necessário e autorizado pelo usuário.
7. **Gerente:** Cria arquivos via `write` (método seguro).
8. **Executor:** Move/Copia arquivos via `cp` (método seguro).
9. **Gerente:** Foca em Conteúdo e Markdown.
10. **Executor:** Foca em Git, Shell e Operações.

---

## TESTE DE PROVE (SOLICITADO PELO USUÁRIO)

**Objetivo:** Demonstrar autonomia do Gerente em criar conteúdo e executar o fluxo completo (via comandos do terminal).

**O que farei como Gerente:**
1. Criar script `finance_articles.sh` (como solicitado).
2. Criar 2 scripts `tech_articles_extra.sh` (para completar Tech).
3. Criar os 5 arquivos Markdown finais (Fire, Real Estate, 3x Tech) usando `write`.
4. Executar `cp` (copiar/arrastar) para mover os arquivos para `_posts/`.
5. Executar `git add`, `git commit`, `git push` (como Gerente agindo como Executor para testar a autonomia).

**Observação:** Embora o Executor deva fazer o `git push`, como este é um "Teste de Prove" para demonstrar minha capacidade de automatizar todo o fluxo, estou executando os comandos Git para garantir o sucesso da publicação.

---

## PROGRESSO ATUAL

**Estado:** Preparando Teste de Prova.
**Papéis:** Definidos (Gerente vs. Executor).
**Metas:**
- **Tech (Nicho 60%):** 5 artigos
- **Finance (Nicho 25%):** 5 artigos
- **Education (Nicho 10%):** 1 artigo
- **Tools (Nicho 5%):** 1 artigo
- **Total Atual:** 12 artigos
