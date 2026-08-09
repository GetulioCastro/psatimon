# AGENTS.MD - Diretrizes de Desenvolvimento e Governança da IA

## 1. Princípios de Governança (SDD - Spec-Driven Development)
- **Especificação é Código**: Nenhuma alteração de funcionalidade deve ser implementada sem especificação/critérios de aceite prévios em documento SPEC.
- **Ciclo de Desenvolvimento Agêntico**: Explore → Plan → Code → Commit/Validate.
- **Validação e Curadoria Humana**: Todo código gerado deve ser aprovado explicitamente. NENHUM push automático ao GitHub/repositório remoto deve ocorrer sem validação humana expressa.

## 2. Restrições de Leitura e Segurança (Guardrails)
- **Arquivos Protegidos**:
  - `.gitignore` (Restrição de leitura e modificação não autorizada)
  - `Agents.md` (Restrição de modificação não autorizada)
- Os agentes de IA estão **estritamente proibidos** de ler, expor ou alterar estes arquivos sensíveis, exceto em fluxos explicitamente autorizados de manutenção do projeto.

## 3. Padrões Visuais e Arquiteturais do Projeto
- **Paleta de Cores Paroquial**:
  - Primária (Destaque/Hover): `#acb1f9`
  - Secundária (Principal/Fundo de Cartões): `#9ba1e8`
- **Manutenção do Padrão Existente**:
  - Respeitar estritamente as classes CSS e a estrutura HTML definida em `index.html` e `style.css`.
  - Responsividade baseada no layout mobile/desktop pré-existente.

## 4. Critérios de Qualidade e Testes de Rejeição
- Todo código HTML/CSS/JS deve passar nos Testes de Rejeição descritos na Mini-Spec antes da homologação.
- Falhas nos testes automatizados ou manuais de rejeição resultarão no bloqueio do deploy/push.
