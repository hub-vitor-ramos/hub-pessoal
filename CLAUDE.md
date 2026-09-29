# CLAUDE.md — hub-pessoal (Landing Page / Portfólio)

Diretrizes para qualquer agente (Claude Code ou outro) trabalhando neste repositório.

## Sobre o projeto
Landing page e portfólio pessoal público. Prioridade: performance, acessibilidade e
first impression visual.

## Regras de UI / Componentes
- Design system: manter tokens de cor, espaçamento e tipografia centralizados
  (ex.: `theme.ts` / `tailwind.config` / `tokens.css`) — nunca hardcode valores mágicos
  espalhados pelos componentes.
- Componentes devem ser responsivos por padrão (mobile-first); testar em pelo menos
  360px, 768px e 1440px de largura antes de considerar concluído.
- Acessibilidade: contraste mínimo AA (WCAG), `alt` em imagens, navegação por teclado
  funcional, elementos semânticos (`<nav>`, `<main>`, `<footer>`, etc.).
- Suporte a tema claro/escuro: nunca fixar cor de fundo/texto sem variante para o outro tema.
- Performance: imagens otimizadas/lazy-loaded, evitar bibliotecas pesadas para efeitos simples.
- Nenhum componente novo deve ser criado sem verificar se já existe um equivalente reutilizável.

## Fluxo de trabalho
- Alterações visuais relevantes devem ser validadas visualmente (screenshot ou preview)
  antes de merge.
- Commits seguem Conventional Commits.
- Mudanças estruturais (novo domínio, nova seção do portfólio) via Pull Request.
