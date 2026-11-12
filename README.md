```markdown
gz‑template
Template de repositório para a Trilha GZ – versionamento, revisão e segurança.

📚 O que é
Projeto base usado nas primeiras semanas da trilha GZ. Ele já contém:

Proteção de branch (main só aceita PRs);
Workflow GitHub Actions com:
release‑please → gera versão SemVer e changelog automaticamente;
gitleaks → impede que segredos sejam commitados.
Estrutura mínima de pastas (.github/workflows) pronta para os próximos módulos (Docker, Supabase, etc.).
🚀 Como usar
```bash
1️⃣ Clone o repositório
git clone https://github.com/SEU_USUARIO/gz-template.git
cd gz-template

2️⃣ (Opcional) Instale dependências do projeto
npm install # ou pip install -r requirements.txt
```

A partir daí você pode criar branches, abrir PRs e deixar o CI fazer o resto.

📦 Versionamento
- Conventional Commits → feat:, fix:, chore: etc.
- SemVer (MAJOR.MINOR.PATCH) é calculado pelo *release‑please* a cada merge na main.
- O changelog é atualizado automaticamente em CHANGELOG.md.

🔒 Segurança
O workflow inclui gitleaks. Se algum commit contiver um segredo (API key, token, senha, etc.), o PR falha e o push é bloqueado.

📄 Licença
Escolha a licença que preferir (ex.: MIT). Basta substituir o texto abaixo ou remover se não for necessário.

```
MIT License

Copyright (c) 2026 <Seu Nome>

Permission is hereby granted, free of charge, to any person obtaining a copy...
```

---

🎯 Por que usar este template?
- Padroniza o fluxo de trabalho da trilha (branch protection, PR obrigatório, CI).
- Ensina a usar *release‑please* e *gitleaks* sem precisar configurar tudo do zero.
- Previne que segredos vazem para o repositório.
- Serve como ponto de partida para os próximos projetos (Docker, Supabase, observabilidade, etc.).

```