# ME Creative

Site profissional e portfólio com atendimento 100% on-line.

Domínio: https://mecreativeprints.com

## Estrutura

- `dist/`: site publicado, imagens e PDFs do portfólio.
- `wrangler.jsonc`: configuração de Cloudflare Workers com arquivos estáticos.
- `package.json`: comandos de validação e publicação.

As imagens e os PDFs são publicados com o site. Nesta versão não há formulário que armazene dados, uploads de visitantes ou banco de dados. O contato abre o WhatsApp ou o e-mail.

## Cloudflare Workers

1. Repositório: `mecreativeprints/me-creative`.
2. Diretório raiz: `/`.
3. Comando de build: `npm run build`.
4. Comando de deploy: `npx wrangler deploy`.
5. Branch de produção: `main`.
6. Nome do Worker: `me-creative`.

A publicação independente depende de autenticar a conta ME Creative no GitHub e a conta proprietária na Cloudflare, concluir o build e confirmar o domínio no Worker. O domínio já está publicado pela hospedagem atual; não troque o destino antes de verificar a publicação independente.

## Execução local

```sh
npm install
npm run build
npm run preview
```

## Atualizações

Os serviços, legendas e traduções estão em `dist/index.html` e `dist/script.js`. A página principal usa português por padrão e oferece inglês, espanhol e polonês. O material de portfólio conserva o idioma da peça original; a versão de demonstração substitui contatos de clientes.

O sitemap está em `https://mecreativeprints.com/sitemap.xml` para envio à propriedade correspondente no Google Search Console.
