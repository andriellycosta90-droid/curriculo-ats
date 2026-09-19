# curriculo-ats
Aplicação web para análise e otimização de currículos para sistemas ATS.

## Sobre o projeto

Muitas empresas utilizam sistemas ATS para analisar e organizar currículos antes que eles sejam avaliados por profissionais de Recursos Humanos. Esses sistemas procuram informações relevantes, como palavras-chave, habilidades, experiências e requisitos relacionados à vaga.

O problema é que um currículo pode ter boas experiências profissionais e ainda assim apresentar baixa compatibilidade com uma vaga por não destacar as informações relevantes da forma adequada.

Esta aplicação foi desenvolvida para facilitar esse processo, permitindo que o usuário informe seu currículo e a descrição da vaga. A aplicação analisa os dois conteúdos, identifica os principais pontos de compatibilidade e gera uma versão do currículo mais adequada à vaga e à leitura por sistemas ATS.

---

## Funcionalidades

* Inserção do currículo pelo usuário;
* Inserção da descrição da vaga;
* Comparação entre currículo e vaga;
* Identificação de palavras-chave e requisitos importantes;
* Análise de compatibilidade;
* Identificação de pontos que podem ser melhorados;
* Geração de uma versão otimizada do currículo;
* Preservação das informações reais do candidato;
* Edição do currículo gerado;
* Exportação do currículo em PDF;
* Interface responsiva;
* Não exige login ou cadastro.

---

## Como utilizar

### 1. Inserir o currículo

O usuário insere o conteúdo do seu currículo na aplicação.

### 2. Inserir a vaga

Em seguida, o usuário cola a descrição da vaga para a qual deseja adaptar o currículo.

### 3. Análise

A aplicação compara as informações do currículo com os requisitos e palavras-chave encontrados na descrição da vaga.

A análise considera aspectos como:

* Experiências profissionais;
* Habilidades;
* Formação;
* Requisitos da vaga;
* Palavras-chave;
* Competências;
* Termos relevantes para ATS.

### 4. Currículo ajustado

Com base na análise, a aplicação gera uma nova versão do currículo, reorganizando e destacando informações relevantes para a vaga.

A aplicação não deve inventar experiências, qualificações ou informações profissionais que não estejam presentes no currículo original.

### 5. Revisão e exportação

O usuário pode revisar e editar o currículo gerado antes de exportá-lo em PDF.

---

# Prompt

O desenvolvimento da aplicação foi orientado por um prompt utilizado no Lovable.

## Versão inicial

```text
Crie uma aplicação web que compare um currículo com uma descrição de vaga e gere uma versão otimizada e ATS Friendly do currículo.

Permita que o usuário cole seu currículo e a descrição da vaga.

Analise a compatibilidade entre currículo e vaga, identificando palavras-chave, habilidades e requisitos importantes.

Gere uma nova versão do currículo otimizada para ATS, sem inventar experiências ou qualificações.

Permita editar o currículo gerado e baixar o resultado em PDF.

Não exigir login ou cadastro.

Utilize uma interface moderna, simples e intuitiva, com paleta principal em tons de vinho, branco e cinza.

O currículo gerado deve possuir estrutura limpa, profissional e compatível com sistemas ATS, evitando tabelas, gráficos, colunas complexas, imagens e elementos que dificultem a leitura automática.
```

## Evolução do prompt

Durante o desenvolvimento, o prompt foi refinado para deixar mais claro o comportamento esperado da aplicação e reduzir ambiguidades.

Foram reforçados principalmente os seguintes pontos:

* A aplicação deveria comparar diretamente o currículo com a vaga;
* A análise deveria identificar palavras-chave e requisitos da vaga;
* O sistema deveria apresentar os pontos de compatibilidade e melhoria;
* O currículo deveria ser adaptado sem inventar informações;
* O resultado deveria manter uma estrutura compatível com ATS;
* O usuário deveria conseguir visualizar e editar o resultado;
* O aplicativo não deveria exigir login;
* O layout deveria utilizar uma identidade visual em tons de vinho.

### Versão final do prompt

```text
Crie uma aplicação web que compare um currículo com uma descrição de vaga e gere uma versão otimizada e ATS Friendly do currículo.

Funcionalidades:
- Permitir que o usuário cole ou envie seu currículo.
- Permitir que o usuário cole a descrição da vaga.
- Analisar a compatibilidade entre currículo e vaga.
- Identificar palavras-chave, habilidades e requisitos importantes presentes na vaga.
- Mostrar um resumo da compatibilidade e os principais pontos que precisam ser melhorados.
- Gerar uma nova versão do currículo otimizada para ATS, sem inventar experiências ou qualificações.
- Permitir editar o currículo gerado.
- Permitir baixar o currículo final em PDF.
- Não exigir login ou cadastro.

Design:
- Interface moderna, simples e intuitiva.
- Paleta principal em tons de vinho, branco e cinza.
- Layout responsivo.
- Currículo com estrutura limpa, profissional e compatível com ATS.
- Evitar tabelas, gráficos, colunas complexas, imagens e elementos que dificultem a leitura por ATS.
```

---

# Como a análise funciona

O fluxo da aplicação foi desenvolvido para seguir quatro etapas principais:

**Currículo → Vaga → Análise → Currículo ajustado**

Primeiramente, o usuário fornece o currículo que deseja analisar.

Depois, insere a descrição da vaga desejada.

A aplicação compara os dois conteúdos e identifica os requisitos, habilidades e palavras-chave relevantes presentes na vaga.

Por fim, utiliza essas informações para gerar uma versão ajustada do currículo, priorizando informações que já existem no currículo original e que possuem relação com a vaga.

O objetivo não é criar informações novas, mas apresentar melhor as experiências e competências que o candidato já possui.

---

# Exemplo de utilização

Para testar a aplicação, foi utilizado um currículo fictício juntamente com uma descrição de vaga fictícia.

O currículo foi inserido na aplicação e, em seguida, foi adicionada a descrição da vaga.

### Currículo utilizado

<img width="717" height="303" alt="image" src="https://github.com/user-attachments/assets/f1e84d5e-49bd-4549-a612-de2df5dbf266" />
<img width="743" height="339" alt="image" src="https://github.com/user-attachments/assets/81b0cc21-5d80-41ad-a62a-4531f11859fc" />
<img width="746" height="274" alt="image" src="https://github.com/user-attachments/assets/72426b28-edf2-4039-b0e9-4c74b1db95f3" />

### Vaga utilizada

<img width="745" height="420" alt="image" src="https://github.com/user-attachments/assets/4f11388c-bd81-4702-a727-e27667fc1521" />
<img width="835" height="484" alt="image" src="https://github.com/user-attachments/assets/d971268c-3f00-4065-a908-d8be139823c8" />

### Resultado da análise

<img width="886" height="492" alt="image" src="https://github.com/user-attachments/assets/a8c2514f-60ea-4c76-a3b4-7a1ec79a80ae" />
<img width="886" height="446" alt="image" src="https://github.com/user-attachments/assets/eb598a34-c141-464d-9002-210d765d11a0" />

### Currículo ajustado

<img width="886" height="508" alt="image" src="https://github.com/user-attachments/assets/fdb1d4bd-2616-4ae1-be25-53f6c69666d6" />

---

# Demonstração da aplicação

<img width="886" height="413" alt="image" src="https://github.com/user-attachments/assets/6a067fa7-78a4-437d-9ec3-465e3105659f" />
<img width="898" height="379" alt="image" src="https://github.com/user-attachments/assets/7d86b54d-ae5e-45dc-bd2d-bfc59d3ce827" />
<img width="886" height="337" alt="image" src="https://github.com/user-attachments/assets/45764c63-ab5a-4377-8d31-da5b36473a4a" />

A aplicação pode ser acessada pelo endereço:

https://resume-craft-311.lovable.app

---

# Tecnologias

A aplicação foi desenvolvida utilizando o Lovable e as tecnologias utilizadas pelo projeto gerado pela plataforma.

---

# Segurança

Nenhuma chave, token, senha ou credencial de acesso deve ser armazenada diretamente no repositório.

---
