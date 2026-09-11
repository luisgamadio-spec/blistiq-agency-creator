# blistiq-agency-creator

Página estática de seleção de produto usada pela Blistiq Agency com a criadora.

- Arquivo único (`index.html`), sem build e sem dependência de servidor.
- O acesso é por link individual: `?t=<token>`. Sem token a página não mostra nada.
- A chave presente no HTML é a chave **anon** do Supabase, pública por desenho.
  Os dados são protegidos por RLS sem policy + funções `security definer` que
  exigem o token do ciclo. Nenhuma credencial administrativa vive aqui.
- Nenhum token de criadora é versionado neste repositório.
