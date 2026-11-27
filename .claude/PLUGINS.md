# Plugins e ferramentas do Claude Code (vídeo "PLUGINS")

## Plugins do Claude Code — já ativados neste repositório (.claude/settings.json)
Ao abrir o Claude Code nesta pasta e confirmar "trust", eles são instalados sozinhos.

| # | Plugin | Para que serve |
|---|--------|----------------|
| 02 | claude-mem@thedotmack | Memória entre sessões (painel em http://localhost:37777) |
| 04 | claude-code-setup@claude-plugins-official | Oficial da Anthropic: analisa o projeto e recomenda hooks, skills, MCP e subagentes (somente leitura) |
| 05 | task-observer@one-skill-to-rule-them-all | Observa as sessões e sugere melhorias nas skills (você aprova antes) |

Para instalar em TODOS os seus projetos (no seu computador), dentro do Claude Code:
```
/plugin marketplace add thedotmack/claude-mem
/plugin install claude-mem@thedotmack
/plugin marketplace add anthropics/claude-plugins-official
/plugin install claude-code-setup@claude-plugins-official
/plugin marketplace add rebelytics/one-skill-to-rule-them-all
/plugin install task-observer@one-skill-to-rule-them-all
```

## Ferramentas externas (não são plugins — instale no seu computador)
### 01 · OmniRoute — gateway que troca de modelo quando o limite acaba (vários modelos grátis)
```
npm install -g omniroute
omniroute            # abre o painel; conecte os provedores e crie um "combo"
```
Depois aponte o Claude Code para o endereço local que o painel mostrar.
Repo: https://github.com/diegosouzapw/OmniRoute

### 03 · Headroom — comprime o contexto para gastar menos tokens
```
pip install headroom-ai
headroom proxy       # inicia o proxy; siga o README para ligar ao Claude Code
```
Repo: https://github.com/chopratejas/headroom
