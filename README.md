# codexa-agent

Repositório de skills do CRM interno da Codexa.

## Skills disponíveis

| Skill | Descrição |
|---|---|
| [codexa-inteligencia-comercial](skills/codexa-inteligencia-comercial/SKILL.md) | Framework de prospecção, qualificação, relacionamento e negociação. |

## Tutorial de instalação

### 1. Obter a skill

Opção A — clonar o repositório:

```bash
git clone https://github.com/gdkdbxwpy6-coder/codexa-agent.git
cd codexa-agent
```

Opção B — baixar apenas o arquivo `skills/codexa-inteligencia-comercial/SKILL.md` pelo botão **Raw** no GitHub e salvá-lo com esse nome.

### 2. Instalar no Claude Code

Crie a pasta da skill no seu diretório de usuário e copie o arquivo:

```bash
mkdir -p ~/.claude/skills/codexa-inteligencia-comercial
cp skills/codexa-inteligencia-comercial/SKILL.md ~/.claude/skills/codexa-inteligencia-comercial/SKILL.md
```

Para instalar apenas em um projeto, use `.claude/skills/` dentro da pasta do projeto em vez de `~/.claude/skills/`.

### 3. Instalar no Claude (app web ou desktop)

1. Compacte a pasta `codexa-inteligencia-comercial` (que deve conter o `SKILL.md`) em um arquivo `.zip`.
2. Abra **Customize → Skills** (ou o equivalente nas configurações da sua versão).
3. Clique em adicionar skill, envie o `.zip` e confirme.

### 4. Verificar a instalação

Em uma nova conversa, peça por exemplo:

> Use a skill codexa-inteligencia-comercial para qualificar este lead: [dados do lead]

Se o Claude citar o framework de pontuação de 0 a 10 e o pipeline da Codexa, a skill está ativa.

## Regras de uso

- A skill não envia mensagens, não contrata serviços e não gera sites sem autorização humana explícita.
- Nota 7 ou mais significa revisão, não permissão de contato.
- Verifique sempre as fontes antes de agir sobre qualquer informação gerada.

## Atualização

Para atualizar, rode `git pull` na pasta clonada e copie o `SKILL.md` novamente para o diretório da skill.
