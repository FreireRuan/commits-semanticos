# commits-semanticos
documentação pessoal sobre commits semânticos


# Convenção de Commits

É de extrema importância adotar convenções consistentes nos commits, pois eles representam confirmações que, quando aplicadas, trarão melhorias ou implementações específicas ao projeto. Cada commit deve ser encarado como uma declaração de propósito, indicando claramente o que será realizado.

Ao utilizar uma convenção padronizada, não apenas promovemos a clareza nas mensagens de commit, mas também facilitamos a compreensão do histórico do projeto por membros da equipe, colaboradores e revisores. A mensagem de commit deve ser escrita de forma imperativa, fornecendo uma instrução direta sobre o que a alteração faz.

Exemplo de uma boa mensagem de commit seguindo a convenção:

```
feat(login): adiciona validação de autenticação de dois fatores

Esta alteração implementa a validação de autenticação de dois fatores durante o processo de login, aprimorando a segurança do sistema.

Resolve #123

```

Neste exemplo, o commit segue a estrutura `<tipo>(<escopo>): <resumo conciso>`, oferecendo informações claras sobre o tipo de alteração, o escopo da modificação e um resumo conciso.

Ao adotar e disseminar práticas de commits consistentes, contribuímos para um versionamento mais organizado e compreensível, beneficiando a colaboração eficiente e o desenvolvimento sustentável do projeto.

### **Padrão de Escrita de Commit:**

```php
<type>(<scope>): <subject>
[body]
[footer]
```

- **`<type>` (Obrigatório):** Indica o tipo de alteração realizada no commit (por exemplo, `fix`, `feat`, `chore`, etc.). Essa parte é obrigatória para que haja clareza sobre o propósito do commit.
- **`(<scope>)` (Opcional):** Indica o escopo da alteração, fornecendo informações adicionais sobre a área ou componente específico do projeto que foi afetado. Essa parte é opcional, dependendo da necessidade de especificar o escopo da alteração.
- **`<subject>` (Obrigatório):** Descreve de maneira concisa o propósito ou a natureza da alteração. É uma parte obrigatória e essencial para entender rapidamente o que o commit realiza.
- **`[body]` (Opcional):** Permite uma descrição mais detalhada das mudanças realizadas. É opcional e geralmente utilizado quando o resumo não é suficiente para transmitir todas as informações necessárias.
- **`[footer]` (Opcional):** Pode incluir informações adicionais, como referências a problemas ou tarefas específicas. Também é opcional e utilizado conforme necessário.

**Exemplo:**

```
fix(login): resolve issue with incorrect user credentials

This commit fixes a bug where the login process failed with incorrect user credentials.

Task #321
```

O uso de partes opcionais depende da necessidade de fornecer informações adicionais ou contextuais sobre a alteração.

### **Convenção de tipo**

- `test`: Indica a adição de novos testes
    - Ex.:  `test: add test for create product automation`
- `feat`: Indica o desenvolvimento de uma feature.
    - Ex.: `feat: implement tracking product service`
- `refactor`: Indica uma refatoração de código.
    - Ex.: `refactor: change return log pattern`
- `style`: Indica a alteração de estilo do código, exemplo: identação…
    - Ex.: `style: change function param for object`
- `fix`: Indica correção de bug de alguma funcionalidade
    - Ex.: `fix: remove getproduct() wrong attribute`
- `chore`: Indica mudanças que não afetam o sistema. Ex.: Regra no gitignore, mudanças pontuais.
    - Ex.: `chore: add no-under role in .gitignore`
- `docs`: Indica alterações relacionas à documentação.
    - Ex.: `docs: add information about list in readme`
- `build`: Indica mudanças que impactam o processo de build do projeto.
    - Ex.: `build: remove pandas dependency`
- `perf`: Indica ajuste de melhoria de performance.
    - Ex.: `perf: change looping for parallel execution`
- `ci`: Indica alteração em processo de ci/cd.
    - Ex.: `ci: add unit test step`
- `revert`: Indica reversão de commits
    - Ex.: `revert: back to aas2525 commit`

### **Convenção de Subject**

O subject deve ser formulado de maneira imperativa, refletindo a ideia de "se aplicado, este commit irá" seguido por uma mensagem imperativa que descreva claramente a ação realizada.

**Exemplo:**

- `Adiciona validação de autenticação de dois fatores`
