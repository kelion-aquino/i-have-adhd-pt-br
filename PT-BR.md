# i-have-adhd-pt-br

Fork do [ayghri/i-have-adhd](https://github.com/ayghri/i-have-adhd) com a skill traduzida para português do Brasil.

A tradução fica em `skills/i-have-adhd-pt-br/`. A pasta original `skills/i-have-adhd/` não foi alterada, para que as atualizações do upstream entrem sem conflito.

## Instalar no Claude Code

```bash
/plugin marketplace add kelion-aquino/i-have-adhd-pt-br
/plugin install i-have-adhd
```

Depois reinicie e chame `/i-have-adhd-pt-br`. Para desligar: "parar modo tdah".

## Instalar no Claude desktop (chat)

Gere o zip. A pasta da skill precisa ficar na raiz do arquivo:

```bash
cd skills && zip -r ../i-have-adhd-pt-br.zip i-have-adhd-pt-br -x "*.DS_Store"
```

Faça o upload de `i-have-adhd-pt-br.zip` nas configurações de skills do app.

## Atualizar a partir do upstream

```bash
git fetch upstream
git merge upstream/main
```

Se o `skills/i-have-adhd/SKILL.md` mudou, compare com `skills/i-have-adhd-pt-br/SKILL.md` e traga as regras novas para o português:

```bash
git diff HEAD...upstream/main -- skills/i-have-adhd/SKILL.md
```
