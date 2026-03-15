<!-- Parte 2/12 (revisada com imagens por URL) — Itens 121–240 -->

## Seção E — Tabelas (GFM) do básico ao “avançado” (121–175)

121) Tabela mínima

**Código:**
```md
| A | B |
|---|---|
| 1 | 2 |
```

**Resultado:**
| A | B |
|---|---|
| 1 | 2 |

---

122) Alinhar coluna à esquerda (padrão)

**Código:**
```md
| Nome | Valor |
|:-----|:------|
| a    | 1     |
```

**Resultado:**
| Nome | Valor |
|:-----|:------|
| a    | 1     |

---

123) Alinhar coluna ao centro

**Código:**
```md
| Nome | Valor |
|:----:|:-----:|
|  a   |   1   |
```

**Resultado:**
| Nome | Valor |
|:----:|:-----:|
|  a   |   1   |

---

124) Alinhar coluna à direita

**Código:**
```md
| Nome | Valor |
|-----:|------:|
| a    |     1 |
```

**Resultado:**
| Nome | Valor |
|-----:|------:|
| a    |     1 |

---

125) Misturar alinhamentos

**Código:**
```md
| Esquerda | Centro | Direita |
|:---------|:------:|--------:|
| a        | b      |       c |
```

**Resultado:**
| Esquerda | Centro | Direita |
|:---------|:------:|--------:|
| a        | b      |       c |

---

126) Tabela com código inline

**Código:**
```md
| Comando | Descrição |
|---|---|
| `npm i` | instala deps |
```

**Resultado:**
| Comando | Descrição |
|---|---|
| `npm i` | instala deps |

---

127) Tabela com bloco de código (tende a NÃO ficar bom no GitHub)

**Código:**
```md
| Exemplo |
|---|
| ```js
| console.log("x")
| ``` |
```

**Resultado:**
| Exemplo |
|---|
| ```js
| console.log("x")
| ``` |

---

128) Alternativa: tabela com `<pre><code>` (HTML)

**Código:**
```html
<table>
  <tr><th>Exemplo</th></tr>
  <tr><td><pre><code>console.log("x")</code></pre></td></tr>
</table>
```

**Resultado:**
<table>
  <tr><th>Exemplo</th></tr>
  <tr><td><pre><code>console.log("x")</code></pre></td></tr>
</table>

---

129) Tabela com links

**Código:**
```md
| Link | Tipo |
|---|---|
| [Docs](https://example.com) | externo |
| [GitHub](https://github.com) | externo |
```

**Resultado:**
| Link | Tipo |
|---|---|
| [Docs](https://example.com) | externo |
| [GitHub](https://github.com) | externo |

---

130) Tabela com imagem pequena (ícone por URL)

**Código:**
```md
| Status | Info |
|---|---|
| ![ok](https://placehold.co/24x24/22c55e/ffffff.png?text=✓) | pronto |
```

**Resultado:**
| Status | Info |
|---|---|
| ![ok](https://placehold.co/24x24/22c55e/ffffff.png?text=✓) | pronto |

---

131) Tabela como “layout” (cards simples)

**Código:**
```md
| Módulo | Descrição |
|---|---|
| **Core** | regras principais |
| **CLI** | interface de linha |
```

**Resultado:**
| Módulo | Descrição |
|---|---|
| **Core** | regras principais |
| **CLI** | interface de linha |

---

132) Tabela com múltiplas linhas (usando `<br>`)

**Código:**
```md
| Campo | Detalhe |
|---|---|
| Observação | Linha 1<br>Linha 2<br>Linha 3 |
```

**Resultado:**
| Campo | Detalhe |
|---|---|
| Observação | Linha 1<br>Linha 2<br>Linha 3 |

---

133) Cabeçalho com 3 colunas

**Código:**
```md
| A | B | C |
|---|---|---|
| 1 | 2 | 3 |
```

**Resultado:**
| A | B | C |
|---|---|---|
| 1 | 2 | 3 |

---

134) “Sem borda” não existe em Markdown; use HTML

**Código:**
```html
<table>
  <tr><td>A</td><td>B</td></tr>
  <tr><td>1</td><td>2</td></tr>
</table>
```

**Resultado:**
<table>
  <tr><td>A</td><td>B</td></tr>
  <tr><td>1</td><td>2</td></tr>
</table>

---

135) Tabela com `<thead>`/`<tbody>`

**Código:**
```html
<table>
  <thead>
    <tr><th>Col</th><th>Val</th></tr>
  </thead>
  <tbody>
    <tr><td>a</td><td>1</td></tr>
  </tbody>
</table>
```

**Resultado:**
<table>
  <thead>
    <tr><th>Col</th><th>Val</th></tr>
  </thead>
  <tbody>
    <tr><td>a</td><td>1</td></tr>
  </tbody>
</table>

---

136) Tabela com `colspan` (HTML)

**Código:**
```html
<table>
  <tr><th colspan="2">Título</th></tr>
  <tr><td>A</td><td>B</td></tr>
</table>
```

**Resultado:**
<table>
  <tr><th colspan="2">Título</th></tr>
  <tr><td>A</td><td>B</td></tr>
</table>

---

137) Tabela com `rowspan` (HTML)

**Código:**
```html
<table>
  <tr><td rowspan="2">Grupo</td><td>Item 1</td></tr>
  <tr><td>Item 2</td></tr>
</table>
```

**Resultado:**
<table>
  <tr><td rowspan="2">Grupo</td><td>Item 1</td></tr>
  <tr><td>Item 2</td></tr>
</table>

---

138) Tabela com alinhamento de célula (HTML)

**Código:**
```html
<table>
  <tr>
    <td align="left">Esq</td>
    <td align="center">Centro</td>
    <td align="right">Dir</td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td align="left">Esq</td>
    <td align="center">Centro</td>
    <td align="right">Dir</td>
  </tr>
</table>

---

139) Tabela com largura (HTML; pode ser ignorado)

**Código:**
```html
<table>
  <tr>
    <td width="60%">Coluna larga</td>
    <td width="40%">Coluna menor</td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td width="60%">Coluna larga</td>
    <td width="40%">Coluna menor</td>
  </tr>
</table>

---

140) Tabela com imagem + texto (agora com URL)

**Código:**
```html
<table>
  <tr>
    <td>
      <img src="https://placehold.co/120x120/111827/ffffff.png?text=LOGO" width="120" alt="Logo">
    </td>
    <td>
      <b>Projeto</b><br>
      Uma descrição curta aqui.
    </td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td>
      <img src="https://placehold.co/120x120/111827/ffffff.png?text=LOGO" width="120" alt="Logo">
    </td>
    <td>
      <b>Projeto</b><br>
      Uma descrição curta aqui.
    </td>
  </tr>
</table>

---

141) “Card” com badge dentro da tabela

**Código:**
```md
| Projeto | Build |
|---|---|
| MeuApp | ![build](https://img.shields.io/badge/build-passing-brightgreen) |
```

**Resultado:**
| Projeto | Build |
|---|---|
| MeuApp | ![build](https://img.shields.io/badge/build-passing-brightgreen) |

---

142) Matriz de compatibilidade

**Código:**
```md
| OS | Suporte |
|---|---|
| Linux | ✅ |
| macOS | ✅ |
| Windows | ⚠️ |
```

**Resultado:**
| OS | Suporte |
|---|---|
| Linux | ✅ |
| macOS | ✅ |
| Windows | ⚠️ |

---

143) Tabela de features

**Código:**
```md
| Feature | Status |
|---|---|
| Login | ✅ |
| Pagamentos | 🚧 |
| Export | ❌ |
```

**Resultado:**
| Feature | Status |
|---|---|
| Login | ✅ |
| Pagamentos | 🚧 |
| Export | ❌ |

---

144) Tabela “estreita” (HTML)

**Código:**
```html
<table>
  <tr><th>Flag</th><th>Desc</th></tr>
  <tr><td><code>-h</code></td><td>ajuda</td></tr>
</table>
```

**Resultado:**
<table>
  <tr><th>Flag</th><th>Desc</th></tr>
  <tr><td><code>-h</code></td><td>ajuda</td></tr>
</table>

---

145) Tabela com âncoras internas (exemplo)

**Código:**
```md
| Seção | Ir |
|---|---|
| Instalação | [#](#instalação) |
| Uso | [#](#uso) |
```

**Resultado:**
| Seção | Ir |
|---|---|
| Instalação | [#](#instalação) |
| Uso | [#](#uso) |

---

146) Tabela com listas dentro (HTML)

**Código:**
```html
<table>
  <tr><th>Tarefas</th></tr>
  <tr>
    <td>
      <ul>
        <li>uma</li>
        <li>duas</li>
      </ul>
    </td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr><th>Tarefas</th></tr>
  <tr>
    <td>
      <ul>
        <li>uma</li>
        <li>duas</li>
      </ul>
    </td>
  </tr>
</table>

---

147) Tabela com `<details>` dentro

**Código:**
```html
<table>
  <tr>
    <td>
      <details>
        <summary>Detalhes</summary>
        Conteúdo escondido.
      </details>
    </td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td>
      <details>
        <summary>Detalhes</summary>
        Conteúdo escondido.
      </details>
    </td>
  </tr>
</table>

---

148) Tabela com `<kbd>`

**Código:**
```md
| Atalho | Ação |
|---|---|
| <kbd>Ctrl</kbd>+<kbd>C</kbd> | copiar |
```

**Resultado:**
| Atalho | Ação |
|---|---|
| <kbd>Ctrl</kbd>+<kbd>C</kbd> | copiar |

---

149) Tabela com `<sub>` e `<sup>`

**Código:**
```md
| Símbolo | Exemplo |
|---|---|
| sub | H<sub>2</sub>O |
| sup | x<sup>2</sup> |
```

**Resultado:**
| Símbolo | Exemplo |
|---|---|
| sub | H<sub>2</sub>O |
| sup | x<sup>2</sup> |

---

150) Roadmap

**Código:**
```md
| Versão | Meta |
|---|---|
| 1.0 | MVP |
| 1.1 | Performance |
| 2.0 | Plugins |
```

**Resultado:**
| Versão | Meta |
|---|---|
| 1.0 | MVP |
| 1.1 | Performance |
| 2.0 | Plugins |

---

151) Changelog compacto

**Código:**
```md
| Data | Mudança |
|---|---|
| 2026-03-15 | docs |
```

**Resultado:**
| Data | Mudança |
|---|---|
| 2026-03-15 | docs |

---

152) Texto longo em tabela

**Código:**
```md
| Campo | Texto |
|---|---|
| Nota | Um texto bem longo que quebra em várias linhas naturalmente. |
```

**Resultado:**
| Campo | Texto |
|---|---|
| Nota | Um texto bem longo que quebra em várias linhas naturalmente. |

---

153) Tabela com `<blockquote>` (HTML)

**Código:**
```html
<table>
  <tr><td><blockquote>Isso é uma citação.</blockquote></td></tr>
</table>
```

**Resultado:**
<table>
  <tr><td><blockquote>Isso é uma citação.</blockquote></td></tr>
</table>

---

154) Imagens alinhadas em tabela (URLs)

**Código:**
```html
<table>
  <tr>
    <td align="center">
      <img src="https://placehold.co/80x80/0ea5e9/ffffff.png?text=A" width="80" alt="A">
    </td>
    <td align="center">
      <img src="https://placehold.co/80x80/f97316/ffffff.png?text=B" width="80" alt="B">
    </td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td align="center">
      <img src="https://placehold.co/80x80/0ea5e9/ffffff.png?text=A" width="80" alt="A">
    </td>
    <td align="center">
      <img src="https://placehold.co/80x80/f97316/ffffff.png?text=B" width="80" alt="B">
    </td>
  </tr>
</table>

---

155) Grid de screenshots (URLs)

**Código:**
```html
<table>
  <tr>
    <td><img src="https://placehold.co/250x140/111827/ffffff.png?text=Screen+1" width="250" alt="Screen 1"></td>
    <td><img src="https://placehold.co/250x140/111827/ffffff.png?text=Screen+2" width="250" alt="Screen 2"></td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td><img src="https://placehold.co/250x140/111827/ffffff.png?text=Screen+1" width="250" alt="Screen 1"></td>
    <td><img src="https://placehold.co/250x140/111827/ffffff.png?text=Screen+2" width="250" alt="Screen 2"></td>
  </tr>
</table>

---

156) Tecnologias com “ícones” (URLs)

**Código:**
```html
<table>
  <tr>
    <td align="center">
      <img src="https://placehold.co/32x32/22c55e/ffffff.png?text=N" width="32" alt="Node"><br>
      Node.js
    </td>
    <td align="center">
      <img src="https://placehold.co/32x32/3b82f6/ffffff.png?text=TS" width="32" alt="TS"><br>
      TypeScript
    </td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td align="center">
      <img src="https://placehold.co/32x32/22c55e/ffffff.png?text=N" width="32" alt="Node"><br>
      Node.js
    </td>
    <td align="center">
      <img src="https://placehold.co/32x32/3b82f6/ffffff.png?text=TS" width="32" alt="TS"><br>
      TypeScript
    </td>
  </tr>
</table>

---

157) Paths em `<code>`

**Código:**
```md
| Arquivo | Função |
|---|---|
| `src/index.ts` | entrypoint |
```

**Resultado:**
| Arquivo | Função |
|---|---|
| `src/index.ts` | entrypoint |

---

158) API endpoints

**Código:**
```md
| Método | Rota | Descrição |
|---|---|---|
| GET | `/health` | status |
| POST | `/login` | autentica |
```

**Resultado:**
| Método | Rota | Descrição |
|---|---|---|
| GET | `/health` | status |
| POST | `/login` | autentica |

---

159) Misturar HTML e texto no `<td>`

**Código:**
```html
<table>
  <tr>
    <td><b>Negrito</b> e <code>código</code></td>
    <td>Texto normal</td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td><b>Negrito</b> e <code>código</code></td>
    <td>Texto normal</td>
  </tr>
</table>

---

160) `<hr>` interno na tabela

**Código:**
```html
<table>
  <tr><td>Parte 1<hr>Parte 2</td></tr>
</table>
```

**Resultado:**
<table>
  <tr><td>Parte 1<hr>Parte 2</td></tr>
</table>

---

161) “Botão” via badge

**Código:**
```md
[![Abrir Docs](https://img.shields.io/badge/Docs-Abrir-blue)](https://example.com)
```

**Resultado:**
[![Abrir Docs](https://img.shields.io/badge/Docs-Abrir-blue)](https://example.com)

---

162) Tabela de comparação

**Código:**
```md
| Opção | Prós | Contras |
|---|---|---|
| A | rápido | simples |
| B | completo | complexo |
```

**Resultado:**
| Opção | Prós | Contras |
|---|---|---|
| A | rápido | simples |
| B | completo | complexo |

---

163) Tabela FAQ (compacta)

**Código:**
```md
| Pergunta | Resposta |
|---|---|
| Funciona? | Sim. |
```

**Resultado:**
| Pergunta | Resposta |
|---|---|
| Funciona? | Sim. |

---

164) Tabela com sinalização

**Código:**
```md
| Nível | Significado |
|---|---|
| 🟢 | ok |
| 🟡 | atenção |
| 🔴 | erro |
```

**Resultado:**
| Nível | Significado |
|---|---|
| 🟢 | ok |
| 🟡 | atenção |
| 🔴 | erro |

---

165) Tabela com SHA “texto”

**Código:**
```md
| Commit | Nota |
|---|---|
| abc123 | fix |
```

**Resultado:**
| Commit | Nota |
|---|---|
| abc123 | fix |

---

166) Tabela “sem cabeçalho” (HTML)

**Código:**
```html
<table>
  <tr><td>A</td><td>B</td></tr>
  <tr><td>1</td><td>2</td></tr>
</table>
```

**Resultado:**
<table>
  <tr><td>A</td><td>B</td></tr>
  <tr><td>1</td><td>2</td></tr>
</table>

---

167) `aria-label` (acessibilidade)

**Código:**
```html
<table aria-label="Tabela de compatibilidade">
  <tr><th>OS</th><th>Suporte</th></tr>
  <tr><td>Linux</td><td>✅</td></tr>
</table>
```

**Resultado:**
<table aria-label="Tabela de compatibilidade">
  <tr><th>OS</th><th>Suporte</th></tr>
  <tr><td>Linux</td><td>✅</td></tr>
</table>

---

168) `<abbr>`

**Código:**
```html
<abbr title="Application Programming Interface">API</abbr>
```

**Resultado:**
<abbr title="Application Programming Interface">API</abbr>

---

169) `<small>`

**Código:**
```html
<small>texto pequeno</small>
```

**Resultado:**
<small>texto pequeno</small>

---

170) `<strong>`

**Código:**
```html
<strong>forte</strong>
```

**Resultado:**
<strong>forte</strong>

---

171) `<em>`

**Código:**
```html
<em>ênfase</em>
```

**Resultado:**
<em>ênfase</em>

---

172) `<del>`

**Código:**
```html
<del>removido</del>
```

**Resultado:**
<del>removido</del>

---

173) `<ins>`

**Código:**
```html
<ins>novo</ins>
```

**Resultado:**
<ins>novo</ins>

---

174) `<mark>`

**Código:**
```html
<mark>destaque</mark>
```

**Resultado:**
<mark>destaque</mark>

---

175) `<code>` + `<kbd>`

**Código:**
```html
Use <kbd>Ctrl</kbd> + <kbd>F</kbd> para buscar em <code>README.md</code>.
```

**Resultado:**
Use <kbd>Ctrl</kbd> + <kbd>F</kbd> para buscar em <code>README.md</code>.

---

## Seção F — Blockquotes (citações) e “callouts” (176–205)

176) Citação simples

**Código:**
```md
> isto é uma citação
```

**Resultado:**
> isto é uma citação

---

177) Citação com negrito

**Código:**
```md
> **Importante:** leia isso.
```

**Resultado:**
> **Importante:** leia isso.

---

178) Citação com itálico

**Código:**
```md
> *observação em itálico*
```

**Resultado:**
> *observação em itálico*

---

179) Citação com link

**Código:**
```md
> Veja [GitHub](https://github.com).
```

**Resultado:**
> Veja [GitHub](https://github.com).

---

180) Citação com lista

**Código:**
```md
> Itens:
> - a
> - b
```

**Resultado:**
> Itens:
> - a
> - b

---

181) Citação com checklist

**Código:**
```md
> - [ ] pendente
> - [x] feito
```

**Resultado:**
> - [ ] pendente
> - [x] feito

---

182) Citação com código

**Código:**
```md
> ```bash
> npm test
> ```
```

**Resultado:**
> ```bash
> npm test
> ```

---

183) Citação aninhada

**Código:**
```md
> Nível 1
>> Nível 2
```

**Resultado:**
> Nível 1
>> Nível 2

---

184) Citação com separador

**Código:**
```md
> texto
> ---
> texto
```

**Resultado:**
> texto
> ---
> texto

---

185) Callout INFO

**Código:**
```md
> ℹ️ **Info:** isso é uma dica.
```

**Resultado:**
> ℹ️ **Info:** isso é uma dica.

---

186) Callout WARNING

**Código:**
```md
> ⚠️ **Atenção:** isso pode quebrar.
```

**Resultado:**
> ⚠️ **Atenção:** isso pode quebrar.

---

187) Callout DANGER

**Código:**
```md
> ❌ **Perigo:** não faça isso em produção.
```

**Resultado:**
> ❌ **Perigo:** não faça isso em produção.

---

188) Callout TIP

**Código:**
```md
> 💡 **Dica:** use `npm ci` no CI.
```

**Resultado:**
> 💡 **Dica:** use `npm ci` no CI.

---

189) Callout NOTE

**Código:**
```md
> 📝 **Nota:** isso é opcional.
```

**Resultado:**
> 📝 **Nota:** isso é opcional.

---

190) Callout com `<details>` dentro

**Código:**
```md
> <details>
>   <summary>Por quê?</summary>
>   Porque sim.
> </details>
```

**Resultado:**
> <details>
>   <summary>Por quê?</summary>
>   Porque sim.
> </details>

---

191) Citação com `<code>`

**Código:**
```md
> Use <code>main</code> como branch.
```

**Resultado:**
> Use <code>main</code> como branch.

---

192) Citação com `<kbd>`

**Código:**
```md
> Atalho: <kbd>Ctrl</kbd> + <kbd>P</kbd>
```

**Resultado:**
> Atalho: <kbd>Ctrl</kbd> + <kbd>P</kbd>

---

193) Citação com `<br>`

**Código:**
```md
> Linha 1<br>
> Linha 2
```

**Resultado:**
> Linha 1<br>
> Linha 2

---

194) Citação com imagem (URL)

**Código:**
```md
> ![Imagem](https://placehold.co/240x120/111827/ffffff.png?text=Imagem)
```

**Resultado:**
> ![Imagem](https://placehold.co/240x120/111827/ffffff.png?text=Imagem)

---

195) Citação com tabela

**Código:**
```md
> | A | B |
> |---|---|
> | 1 | 2 |
```

**Resultado:**
> | A | B |
> |---|---|
> | 1 | 2 |

---

196) `<blockquote>` direto

**Código:**
```html
<blockquote>Texto em blockquote.</blockquote>
```

**Resultado:**
<blockquote>Texto em blockquote.</blockquote>

---

197) Limite: CSS/JS não controlado no README

**Código:**
```md
<!-- Sem JS e sem CSS externo no README do GitHub. -->
```

**Resultado:**
<!-- Sem JS e sem CSS externo no README do GitHub. -->

---

198) Callout com badge

**Código:**
```md
> ![status](https://img.shields.io/badge/status-beta-yellow)
```

**Resultado:**
> ![status](https://img.shields.io/badge/status-beta-yellow)

---

199) Callout com badge clicável

**Código:**
```md
> [![Docs](https://img.shields.io/badge/docs-open-blue)](https://example.com)
```

**Resultado:**
> [![Docs](https://img.shields.io/badge/docs-open-blue)](https://example.com)

---

200) Citação com heading

**Código:**
```md
> ### Título dentro da citação
> Texto
```

**Resultado:**
> ### Título dentro da citação
> Texto

---

201) Citação com lista numerada

**Código:**
```md
> 1. passo 1
> 2. passo 2
```

**Resultado:**
> 1. passo 1
> 2. passo 2

---

202) Citação com código inline

**Código:**
```md
> `inline code`
```

**Resultado:**
> `inline code`

---

203) Citação com setas

**Código:**
```md
> ➜ siga para a próxima seção
```

**Resultado:**
> ➜ siga para a próxima seção

---

204) Citação e texto normal

**Código:**
```md
> citação

texto normal fora da citação
```

**Resultado:**
> citação

texto normal fora da citação

---

205) Citação para “saída esperada”

**Código:**
```md
> Saída esperada:
> ```
> OK
> DONE
> ```
```

**Resultado:**
> Saída esperada:
> ```
> OK
> DONE
> ```

---

## Seção G — `<details>` / `<summary>` (spoilres/acordeão) (206–240)

206) Details básico

**Código:**
```html
<details>
  <summary>Mostrar</summary>
  Conteúdo escondido.
</details>
```

**Resultado:**
<details>
  <summary>Mostrar</summary>
  Conteúdo escondido.
</details>

---

207) Details com parágrafos

**Código:**
```html
<details>
  <summary>Detalhes</summary>

  Parágrafo 1.

  Parágrafo 2.
</details>
```

**Resultado:**
<details>
  <summary>Detalhes</summary>

  Parágrafo 1.

  Parágrafo 2.
</details>

---

208) Details com lista

**Código:**
```html
<details>
  <summary>Lista</summary>

  - a
  - b
</details>
```

**Resultado:**
<details>
  <summary>Lista</summary>

  - a
  - b
</details>

---

209) Details com checklist

**Código:**
```html
<details>
  <summary>Tarefas</summary>

  - [ ] uma
  - [x] duas
</details>
```

**Resultado:**
<details>
  <summary>Tarefas</summary>

  - [ ] uma
  - [x] duas
</details>

---

210) Details com código

**Código:**
```html
<details>
  <summary>Código</summary>

  ```bash
  npm ci
  ```
</details>
```

**Resultado:**
<details>
  <summary>Código</summary>

  ```bash
  npm ci
  ```
</details>

---

211) Details com múltiplos blocos

**Código:**
```html
<details>
  <summary>Mais</summary>

  Texto.

  ```js
  console.log("a");
  ```

  ```ts
  const x: number = 1;
  ```
</details>
```

**Resultado:**
<details>
  <summary>Mais</summary>

  Texto.

  ```js
  console.log("a");
  ```

  ```ts
  const x: number = 1;
  ```
</details>

---

212) Details com tabela

**Código:**
```html
<details>
  <summary>Tabela</summary>

  | A | B |
  |---|---|
  | 1 | 2 |
</details>
```

**Resultado:**
<details>
  <summary>Tabela</summary>

  | A | B |
  |---|---|
  | 1 | 2 |
</details>

---

213) Details com imagem (URL)

**Código:**
```html
<details>
  <summary>Screenshot</summary>

  <img src="https://placehold.co/600x280/111827/ffffff.png?text=Screenshot" width="600" alt="s1">
</details>
```

**Resultado:**
<details>
  <summary>Screenshot</summary>

  <img src="https://placehold.co/600x280/111827/ffffff.png?text=Screenshot" width="600" alt="s1">
</details>

---

214) Details FAQ

**Código:**
```html
<details>
  <summary>Isso funciona no GitHub?</summary>

  Sim, <code>&lt;details&gt;</code> costuma funcionar em README.
</details>
```

**Resultado:**
<details>
  <summary>Isso funciona no GitHub?</summary>

  Sim, <code>&lt;details&gt;</code> costuma funcionar em README.
</details>

---

215) Vários details em sequência

**Código:**
```html
<details><summary>P1</summary>R1</details>
<details><summary>P2</summary>R2</details>
```

**Resultado:**
<details><summary>P1</summary>R1</details>
<details><summary>P2</summary>R2</details>

---

216) Details com `<br>`

**Código:**
```html
<details>
  <summary>Ver</summary>
  Linha 1<br>
  Linha 2
</details>
```

**Resultado:**
<details>
  <summary>Ver</summary>
  Linha 1<br>
  Linha 2
</details>

---

217) Details com blockquote interno

**Código:**
```html
<details>
  <summary>Citação</summary>

  > citação aqui
</details>
```

**Resultado:**
<details>
  <summary>Citação</summary>

  > citação aqui
</details>

---

218) Details com `<pre><code>`

**Código:**
```html
<details>
  <summary>Saída</summary>
  <pre><code>OK
DONE</code></pre>
</details>
```

**Resultado:**
<details>
  <summary>Saída</summary>
  <pre><code>OK
DONE</code></pre>
</details>

---

219) Details com `<kbd>`

**Código:**
```html
<details>
  <summary>Atalhos</summary>

  <kbd>Ctrl</kbd> + <kbd>S</kbd>
</details>
```

**Resultado:**
<details>
  <summary>Atalhos</summary>

  <kbd>Ctrl</kbd> + <kbd>S</kbd>
</details>

---

220) Details com links

**Código:**
```html
<details>
  <summary>Links</summary>

  - <a href="https://example.com">Docs</a>
  - <a href="https://github.com">GitHub</a>
</details>
```

**Resultado:**
<details>
  <summary>Links</summary>

  - <a href="https://example.com">Docs</a>
  - <a href="https://github.com">GitHub</a>
</details>

---

221) Summary chamativo

**Código:**
```html
<details>
  <summary><b>CLI — opções avançadas</b></summary>

  Conteúdo.
</details>
```

**Resultado:**
<details>
  <summary><b>CLI — opções avançadas</b></summary>

  Conteúdo.
</details>

---

222) Emoji no summary

**Código:**
```html
<details>
  <summary>⚙️ Configurações</summary>

  Conteúdo.
</details>
```

**Resultado:**
<details>
  <summary>⚙️ Configurações</summary>

  Conteúdo.
</details>

---

223) Summary com `<br>` (varia)

**Código:**
```html
<details>
  <summary>Primeira linha<br>Segunda linha</summary>
  Conteúdo.
</details>
```

**Resultado:**
<details>
  <summary>Primeira linha<br>Segunda linha</summary>
  Conteúdo.
</details>

---

224) Details com `<ul>`

**Código:**
```html
<details>
  <summary>HTML list</summary>
  <ul>
    <li>um</li>
    <li>dois</li>
  </ul>
</details>
```

**Resultado:**
<details>
  <summary>HTML list</summary>
  <ul>
    <li>um</li>
    <li>dois</li>
  </ul>
</details>

---

225) Details dentro de tabela

**Código:**
```html
<table>
  <tr>
    <td>
      <details>
        <summary>Detalhes</summary>
        Conteúdo.
      </details>
    </td>
  </tr>
</table>
```

**Resultado:**
<table>
  <tr>
    <td>
      <details>
        <summary>Detalhes</summary>
        Conteúdo.
      </details>
    </td>
  </tr>
</table>

---

226) Changelog escondido

**Código:**
```html
<details>
  <summary>Changelog completo</summary>

  - 1.0.0: inicial
  - 1.1.0: melhorias
</details>
```

**Resultado:**
<details>
  <summary>Changelog completo</summary>

  - 1.0.0: inicial
  - 1.1.0: melhorias
</details>

---

227) Stack trace (texto)

**Código:**
```html
<details>
  <summary>Stack trace</summary>

  ```text
  Error: x
    at y
  ```
</details>
```

**Resultado:**
<details>
  <summary>Stack trace</summary>

  ```text
  Error: x
    at y
  ```
</details>

---

228) Logs

**Código:**
```html
<details>
  <summary>Logs</summary>

  ```log
  [INFO] ok
  ```
</details>
```

**Resultado:**
<details>
  <summary>Logs</summary>

  ```log
  [INFO] ok
  ```
</details>

---

229) Variáveis de ambiente

**Código:**
```html
<details>
  <summary>ENV</summary>

  ```env
  NODE_ENV=production
  ```
</details>
```

**Resultado:**
<details>
  <summary>ENV</summary>

  ```env
  NODE_ENV=production
  ```
</details>

---

230) Details “apertado”

**Código:**
```html
<details><summary>Ok</summary>Conteúdo sem quebras pode ficar apertado.</details>
```

**Resultado:**
<details><summary>Ok</summary>Conteúdo sem quebras pode ficar apertado.</details>

---

231) Details “bonito” com espaçamento

**Código:**
```html
<details>
  <summary>Ok</summary>

  Conteúdo com melhor leitura.
</details>
```

**Resultado:**
<details>
  <summary>Ok</summary>

  Conteúdo com melhor leitura.
</details>

---

232) Banner ASCII

**Código:**
```html
<details>
  <summary>Banner</summary>

  ```text
  ==========
   PROJETO
  ==========
  ```
</details>
```

**Resultado:**
<details>
  <summary>Banner</summary>

  ```text
  ==========
   PROJETO
  ==========
  ```
</details>

---

233) Preview com imagem (URL)

**Código:**
```html
<details>
  <summary>Ver preview</summary>

  <img src="https://placehold.co/720x320/111827/ffffff.png?text=Preview" width="720" alt="preview">
</details>
```

**Resultado:**
<details>
  <summary>Ver preview</summary>

  <img src="https://placehold.co/720x320/111827/ffffff.png?text=Preview" width="720" alt="preview">
</details>

---

234) Spoiler

**Código:**
```html
<details>
  <summary>spoiler</summary>
  O vilão era o jardineiro.
</details>
```

**Resultado:**
<details>
  <summary>spoiler</summary>
  O vilão era o jardineiro.
</details>

---

235) FAQ compatibilidade

**Código:**
```html
<details>
  <summary>Windows é suportado?</summary>
  Parcialmente.
</details>
```

**Resultado:**
<details>
  <summary>Windows é suportado?</summary>
  Parcialmente.
</details>

---

236) FAQ licença

**Código:**
```html
<details>
  <summary>Qual a licença?</summary>
  Veja <a href="https://example.com">LICENSE</a>.
</details>
```

**Resultado:**
<details>
  <summary>Qual a licença?</summary>
  Veja <a href="https://example.com">LICENSE</a>.
</details>

---

237) Como contribuir

**Código:**
```html
<details>
  <summary>Como contribuir</summary>

  1. Fork
  2. Branch
  3. PR
</details>
```

**Resultado:**
<details>
  <summary>Como contribuir</summary>

  1. Fork
  2. Branch
  3. PR
</details>

---

238) Código de conduta

**Código:**
```html
<details>
  <summary>Código de conduta</summary>

  Seja respeitoso.
</details>
```

**Resultado:**
<details>
  <summary>Código de conduta</summary>

  Seja respeitoso.
</details>

---

239) Mermaid dentro do details

**Código:**
```html
<details>
  <summary>Diagrama</summary>

  ```mermaid
  flowchart LR
    A --> B
  ```
</details>
```

**Resultado:**
<details>
  <summary>Diagrama</summary>

  ```mermaid
  flowchart LR
    A --> B
  ```
</details>

---

240) Resumo em lista

**Código:**
```html
<details>
  <summary>Resumo</summary>

  - objetivo
  - instalação
  - uso
</details>
```

**Resultado:**
<details>
  <summary>Resumo</summary>

  - objetivo
  - instalação
  - uso
</details>
