# Protecwork Hub

Aplicação web estática pronta para publicação no GitHub Pages.

## Arquivos

- `index.html`: aplicação completa, com o importador local de certificados PDF e os cabeçalhos temáticos incorporados.
- `assets/`: imagens dos cabeçalhos das normas, mantidas como assets reutilizáveis.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub.
2. Envie `index.html` para a raiz do repositório. A pasta `assets` é opcional para o funcionamento atual, pois as imagens já estão incorporadas no HTML, mas foi incluída no pacote para organização e reutilização.
3. No repositório, abra **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch principal e a pasta `/ (root)`.
6. Salve e aguarde o endereço do GitHub Pages ficar disponível.

A aplicação usa as bibliotecas PDF.js, jsPDF, AutoTable e Supabase por CDN. Portanto, o site precisa ser acessado por HTTPS no GitHub Pages para que os recursos externos funcionem corretamente.

## Funcionalidades incluídas

- Importação múltipla de certificados PDF diretamente no navegador.
- Revisão e correção dos dados antes da importação.
- Cadastro automático em certificados e controle de vencimentos.
- Geração de certificados em PDF com frente e verso.
- Cabeçalhos temáticos para NR-05, NR-06, NR-10, NR-11, NR-12, NR-18, NR-23, NR-33, NR-34 e NR-35.
- Persistência e autenticação via Supabase já configuradas no aplicativo.

Não renomeie o arquivo `index.html` e não altere as constantes de configuração do Supabase se quiser manter a conexão com a base atual.
