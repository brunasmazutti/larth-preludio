# LARTH — Prelúdio

Experiência digital de presente da LARTH Beauté + ferramenta interna de geração de links personalizados.

## Arquivos

- **`index.html`** — a experiência que a cliente recebe (o "Prelúdio").
- **`admin.html`** — ferramenta interna, só para a equipe. Gera o link personalizado com os nomes de quem presenteia e quem recebe.
- **`404.html`** — arquivo técnico. Faz os links "limpos" (`larth.com.br/CODIGO`) funcionarem no GitHub Pages. Não precisa mexer nele.
- **`CNAME`** — indica o domínio próprio (`larth.com.br`). Edite ou apague este arquivo se o domínio final for outro.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (pode ser público ou privado, mas privado exige um plano pago do GitHub para usar o Pages).
2. Envie estes 4 arquivos (`index.html`, `admin.html`, `404.html`, `CNAME`) para a raiz do repositório.
3. No repositório, vá em **Settings → Pages**.
4. Em "Source", selecione a branch `main` e a pasta `/root`. Salve.
5. Aguarde alguns minutos — o GitHub vai te dar um endereço tipo `usuario.github.io/nome-do-repositorio`.

### Se for usar o domínio próprio (`larth.com.br`)

6. Ainda em **Settings → Pages**, no campo "Custom domain", digite `larth.com.br` (ou o domínio real).
7. No painel onde o domínio `larth.com.br` está registrado (GoDaddy, Registro.br, Hostinger, etc.), configure os registros DNS conforme a própria tela do GitHub indicar (geralmente registros do tipo `A` apontando para os servidores do GitHub, ou um `CNAME` se for subdomínio).
8. Isso pode levar algumas horas para propagar.

### Se **não** for usar domínio próprio ainda

Sem problema — o site já funciona no endereço padrão do GitHub (`usuario.github.io/nome-do-repositorio`). Só que, nesse caso, os links "limpos" ficam assim: `usuario.github.io/nome-do-repositorio/CODIGO` (com o nome do repositório no meio) — ainda funciona perfeitamente, só não fica tão enxuto quanto com domínio próprio.

## Como a equipe usa no dia a dia

1. Abra o `admin.html` (é a ferramenta interna — não compartilhe esse link com clientes).
2. Preencha o nome de quem está presenteando e de quem vai receber.
3. Clique em "Gerar link".
4. Copie o link ou clique em "Enviar no WhatsApp" para mandar direto para quem comprou o presente.
5. Quem comprou reenvia a mensagem, sem precisar editar nada — ela já não tem nenhum spoiler.

## Observação importante

Os nomes não ficam escritos de forma legível no link (vão codificados). Isso evita que apareçam por acidente na tela de alguém antes da hora — mas não é uma criptografia forte, apenas ofuscação básica. Não é recomendado para dados sensíveis, apenas para preservar a surpresa do presente.
