# Portfólio — Joaquim Paulo Vieira de Melo

Site estático com o portfólio pessoal.

## Estrutura do projeto

- `index.html` — página principal
- `style.css` — estilos
- `img/` — imagens (ex.: `foto-perfil.jfif`)

## Como usar localmente

Basta abrir o `index.html` no navegador. Para testar rápido via terminal (PowerShell):

```powershell
# abrir com o navegador padrão (Windows)
Start-Process -FilePath "index.html"
```

Ou iniciar um servidor local simples (útil para APIs/paths relativos):

```powershell
# usando Python 3 (se instalado)
cd 'c:\Users\joaqu\3D Objects\coding\portifolio'
python -m http.server 8000
# depois abra http://localhost:8000
```

## Inicializar repositório Git local

Execute os comandos abaixo no PowerShell dentro do diretório `c:\Users\joaqu\3D Objects\coding\portifolio`:

```powershell
cd 'c:\Users\joaqu\3D Objects\coding\portifolio'
# inicializar repositório
git init
# forçar branch principal para 'main' quando necessário
git branch -M main
# adicionar arquivos e commitar
git add .
git commit -m "Initial commit: website, README and .gitignore"
```

## Criar repositório remoto e enviar (push)

Opção 1 — Pelo site do GitHub:
- Crie um novo repositório no GitHub (por exemplo `joaquim-portfolio`).
- Copie a URL HTTPS do repositório e execute:

```powershell
# substituir <USERNAME> e <REPO> pela sua conta e repo
git remote add origin https://github.com/<USERNAME>/<REPO>.git
git push -u origin main
```

Opção 2 — Usando a CLI `gh` (se instalada):

```powershell
# cria repo público e faz push do conteúdo atual
gh repo create <USERNAME>/<REPO> --public --source=. --remote=origin --push
```

## Deploy (GitHub Pages)

- No GitHub, vá em `Settings` → `Pages` e escolha a branch `main` e a pasta `/ (root)`.
- Aguarde alguns minutos e o site estará disponível em `https://<USERNAME>.github.io/<REPO>/`.

Alternativas: Netlify ou Vercel (basta apontar para o repositório e configurar deploy automático).

## Licença (recomendado)

Se quiser permitir uso aberto, adicione um `LICENSE` com a licença MIT. Exemplo rápido:

```powershell
# criar arquivo LICENSE com texto MIT (ou usar a interface do GitHub)
```

## Contato

Email: `joaquimpaulovieirademeloo@gmail.com`

---

Se quiser, eu posso:
- criar o `LICENSE` (MIT) aqui;
- inicializar o `git` e executar o commit para você;
- gerar os passos exatos para criar o repo remoto ou gerar o comando `gh repo create` pronto para colar.
