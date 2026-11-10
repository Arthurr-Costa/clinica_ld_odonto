# L&D Odonto — Site institucional

Site institucional da **L&D Odonto**, desenvolvido para apresentar a clínica, divulgar suas especialidades e facilitar o contato para agendamento de avaliações.

🔗 **[Acesse o site](https://arthurr-costa.github.io/clinica_ld_odonto/)**

## Sobre o projeto

A página apresenta os serviços e a proposta de atendimento da clínica em uma interface responsiva, com navegação para dispositivos móveis e contato direto pelo WhatsApp.

O projeto utiliza **HTML, CSS e JavaScript puros**, sem necessidade de backend ou banco de dados. Os agendamentos são encaminhados ao WhatsApp da clínica.

Este repositório também é utilizado em uma atividade acadêmica sobre versionamento, colaboração e publicação de software com GitHub, com autorização da professora para utilizar um projeto existente.

## Funcionalidades

- Apresentação institucional da clínica.
- Divulgação de especialidades odontológicas.
- Contato para agendamento pelo WhatsApp.
- Seção de dúvidas frequentes.
- Links para Instagram e WhatsApp.
- Menu de navegação para dispositivos móveis.
- Animações de entrada com suporte à preferência por movimento reduzido.
- Atualização automática do ano no rodapé.

## Tecnologias

| Tecnologia | Finalidade |
| --- | --- |
| HTML5 | Estrutura e conteúdo |
| CSS3 | Estilização, responsividade e animações |
| JavaScript | Interações da interface |
| Git e GitHub | Versionamento e colaboração |
| GitHub Actions | Automação dos workflows |
| GitHub Pages | Hospedagem do site |

## Estrutura do projeto

| Arquivo | Responsabilidade |
| --- | --- |
| `index.html` | Estrutura e conteúdo da página |
| `styles.css` | Estilos e comportamento responsivo |
| `script.js` | Menu, cabeçalho e animações |
| `.github/workflows/blank.yml` | Workflow inicial de CI |
| `.github/workflows/static.yml` | Publicação no GitHub Pages |
| `LICENSE` | Licença do projeto |

> O HTML referencia imagens e ícones em `assets/`. Esses arquivos precisam estar disponíveis nos caminhos indicados para o carregamento correto dos recursos.

## Como executar localmente

### Pré-requisitos

- Git.
- Navegador atualizado.
- Python 3 para utilizar o servidor local abaixo, ou a extensão Live Server do VS Code.

### 1. Clone o repositório

```bash
git clone https://github.com/Arthurr-Costa/clinica_ld_odonto.git
cd clinica_ld_odonto
```

### 2. Inicie o servidor local

```bash
python -m http.server 8000
```

No Windows, também é possível utilizar:

```bash
py -m http.server 8000
```

No macOS ou Linux:

```bash
python3 -m http.server 8000
```

### 3. Acesse no navegador

Abra **http://localhost:8000**.

Para encerrar o servidor, pressione **Ctrl + C** no terminal.

## Acessibilidade

O código inclui:

- Idioma definido como português do Brasil.
- Link para pular ao conteúdo principal.
- Estrutura com elementos semânticos.
- Texto alternativo nas imagens informativas.
- Estado do menu móvel informado por `aria-expanded`.
- Animações que consideram `prefers-reduced-motion`.

A navegação por teclado, o contraste e o comportamento com leitores de tela devem ser verificados durante a evolução do projeto.

## Automação e publicação

A hospedagem utiliza o **GitHub Pages**, com publicação pelo **GitHub Actions**.

| Workflow | Comportamento atual |
| --- | --- |
| `blank.yml` | Executa no push e em Pull Requests para `main`; contém comandos de exemplo, sem testes automatizados |
| `static.yml` | Publica o site após push para `main` ou execução manual |

Os workflows podem ser acompanhados na aba [Actions](https://github.com/Arthurr-Costa/clinica_ld_odonto/actions).

Em **Settings → Pages**, a origem da publicação deve estar configurada como **GitHub Actions**.

> Atualmente, a publicação e o CI são independentes. O deploy ainda não depende da aprovação de testes automatizados.

## Fluxo de contribuição

1. Abra uma Issue descrevendo o problema ou a melhoria.
2. Crie uma branch a partir da `main`.
3. Implemente a alteração e valide localmente.
4. Registre commits com mensagens claras.
5. Abra um Pull Request explicando a mudança e a validação realizada.
6. Utilize `Closes #NUMERO` na descrição do PR quando houver uma Issue a encerrar.
7. Após a revisão e o merge, acompanhe o deploy e confira o site publicado.


## Autor

**Arthur Costa**

[Perfil no GitHub](https://github.com/Arthurr-Costa)

## Licença

Este projeto utiliza a licença **MIT**. Consulte [LICENSE](LICENSE) para mais informações.
