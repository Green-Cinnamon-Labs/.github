# Linha Governança

Issues da org inteira, em `Green-Cinnamon-Labs/.github` (#1 a #10). A ordem recomendada é a dos números. O método é o mesmo das outras linhas (ver `../spec-hefesto/WORKFLOW.md`).

- Quem aplica as configurações é o usuário: rulesets, opções de merge, segurança, labels, topics, board. Nunca altere configurações da org ou dos repositórios (`gh api` com PATCH, POST, PUT ou DELETE, `gh repo edit`, `gh label`, etc.). Leitura com `gh` é livre.
- Os arquivos deste repositório (`GOVERNANCE.md`, templates, workflows, scripts) também são do usuário. Só edite o `CLAUDE.md` e o perfil, quando ele pedir.
- Guie por versão: "o que está assim hoje → mude para → por quê (1 a 3 linhas)", e depois como conferir (de preferência com um `gh api` de leitura).
- Todo conceito novo vem com a genealogia: quando surgiu, que problema o forçou a existir, o que ele corrige da solução anterior. Nunca regras soltas.
- Org no plano Free: rulesets só em repositórios públicos; ruleset da org inteira exige Team; os privados do Sísifo ficam sem rulesets e sem secret scanning.
- Seja objetivo: sem recaps e sem listas de próximos passos.
- Commits em Conventional Commits, em inglês, com `Refs #N`.
- Fechamento só quando o usuário disser "close-out": comentário na issue e texto do PR.

## Um chat por issue

O usuário abre um chat para cada issue, nesta pasta. Ao começar:

1. Leia a issue e os comentários (`gh issue view <n> -R Green-Cinnamon-Labs/.github --comments`) e as issues citadas em "Depende de".
2. Descubra em que versão o usuário está: os itens marcados no checklist, os comentários de versão, a branch e os commits da issue (`git log --oneline`) e o estado real da configuração no GitHub.
3. Se faltar alguma dependência, avise antes de começar.
4. Comece a guiar pela próxima versão não marcada.
