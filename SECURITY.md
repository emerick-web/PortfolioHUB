# Política de Segurança — PortfolioHUB

Este documento define as diretrizes de segurança, práticas recomendadas e os procedimentos para o reporte de vulnerabilidades no projeto **PortfolioHUB**.

---

## 🚀 Versões Suportadas

Como o PortfolioHUB é um site estático hospedado publicamente, apenas a versão mais recente e integrada à branch principal (`main`) recebe suporte e atualizações ativas.

| Versão | Suportada | Notas |
| :--- | :---: | :--- |
| `v1.x` (Atual/`main`) |  Sim | Versão ativa de produção no GitHub Pages. |
| `< v1.0` | ❌ Não | Versões de desenvolvimento antigo ou ramificações obsoletas. |

---

## 🔒 Práticas de Segurança Adotadas

Para garantir a integridade do portfólio e mitigar riscos de acessos não autorizados, o repositório adota as seguintes camadas de proteção:

*   **Autenticação de Dois Fatores (2FA):** Exigida rigorosamente para a conta do proprietário e de quaisquer colaboradores com acesso de escrita.
*   **Proteção de Branch (`main`):** Configurada via GitHub Rulesets. É estritamente proibido realizar `push` direto na ramificação principal. Qualquer alteração deve, obrigatoriamente, ser submetida por meio de uma branch secundária (`feature/*`) e integrada exclusivamente via *Pull Request*.
*   **Tokens com Escopo Mínimo:** Tokens de Acesso Pessoal (PATs) eventualmente utilizados seguem o princípio do menor privilégio, limitando os escopos estritamente ao necessário.

---

## 👥 Política de Acesso a Colaboradores

O controle de privilégios dentro do ecossistema do projeto é dividido em níveis claros de responsabilidade:

*   **Proprietário (Admin):** Controle total sobre as configurações de infraestrutura, gerenciamento do GitHub Pages e políticas de segurança.
*   **Colaboradores externos (Write):** Permissão restrita para sugerir melhorias. O fluxo exige a criação de forks/branches e validação manual do código antes do merge.
*   **Público Geral (Read):** Acesso estrito de leitura para auditoria e visualização do portfólio.

---

## ⚠️ Como Reportar Vulnerabilidades

Se você identificar qualquer falha de segurança, brecha de exposição ou potencial risco neste projeto, **por favor, não abra uma Issue pública**. 

Para realizar um reporte seguro e responsável, siga o fluxo abaixo:

1. Envie um e-mail detalhado diretamente para: **enzoemerick@sempreceub.com**
2. No corpo da mensagem, inclua:
    * Uma descrição clara da vulnerabilidade encontrada.
    * O passo a passo ou código necessário para reproduzir a falha (PoC).
    * O impacto potencial que a falha pode causar ao ambiente.

Agradecemos a colaboração para manter este projeto seguro! Uma resposta com o plano de correção será enviada em até 48 horas úteis.
