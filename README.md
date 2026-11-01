# Modelagem de Ameaças

Site educativo, em HTML e CSS, que explica o que é modelagem de ameaças e por que aplicá-la desde o início do desenvolvimento de software.

## O que o site aborda

- O que é modelagem de ameaças e como pensar do ponto de vista de um invasor.
- Por que corrigir uma falha em produção custa muito mais do que preveni-la na concepção.
- As quatro etapas do processo:
  1. Avaliar e diagramar a aplicação.
  2. Identificar falhas de segurança.
  3. Corrigir as falhas.
  4. Verificar se as correções funcionam.

## Exemplo tratado no site

Em um diagrama, percebe-se que a comunicação entre o banco de dados e o servidor web não usa TLS. Assim, um invasor poderia se passar pelo banco de dados. A mitigação é configurar TLS ou, melhor ainda, mTLS, em que os dois lados verificam a identidade um do outro.

## Como executar

Não há instalação nem etapa de build.

```bash
git clone https://github.com/dilione-junior/modelagem.git
cd modelagem
python -m http.server 8000
```

Depois, acesse `http://localhost:8000`. Se preferir, abra o arquivo `index.html` diretamente no navegador.

## Estrutura

```text
index.html          Conteúdo da página
estilos/styles.css  Estilos
imagens/            Imagens usadas no conteúdo
```

## Para saber mais

- [Threat Modeling Process, da OWASP](https://owasp.org/www-community/Threat_Modeling_Process)

Desenvolvido por Dilione Junior.
