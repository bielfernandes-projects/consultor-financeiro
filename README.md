# consultor-financeiro

Skill de consultor financeiro pessoal para Claude Code. Lê minha vida financeira
de arquivos locais (`perfil.md`, `historico.md`, planilhas exportadas) e dá
recomendação com a aritmética na mesa. Contexto Brasil / BRL.

## Instalar em outra máquina

```bash
git clone https://github.com/bielfernandes-projects/consultor-financeiro.git
cp -r consultor-financeiro ~/.claude/skills/consultor-financeiro
```

Depois, ajuste o caminho da pasta de dados no topo do `SKILL.md` se nessa
máquina ele for diferente, e crie a estrutura:

```
<pasta de dados>/
  planilhas/            exports financas_AAAA-MM-DD.xlsx
  perfil.md
  historico.md
```

Requer Python com `openpyxl` (`pip install openpyxl`) para ler as planilhas.

## Importante

Os dados financeiros (`perfil.md`, `historico.md`, planilhas, roadmaps) moram
**fora deste repo** e nunca são commitados. Só a skill vive aqui.
