# Challenge: Panama Papers & The Islandic Crisis

## 📋 Informações
- **Categoria:** OSINT (Open Source Intelligence)
- **Plataforma:** HackTheBox
- **Dificuldade:** Fácil

---

## 📖 Descrição do Desafio
Este pequeno país sofreu com resgates e dívidas após o colapso bancário de 2008. A descoberta de que um político importante e sua esposa estavam ligados a uma empresa offshore vinculada a bancos falidos gerou protestos massivos e sua renúncia em menos de 48 horas. Foi o primeiro grande líder a cair com o vazamento dos Panama Papers.

**Objetivos:**
1. Identificar o nome da empresa offshore vinculada.
2. Identificar o nome completo da esposa do político.
3. Identificar o período oficial da vinculação.

---

## 🔍 Investigação e Enumeração

### 1. Coleta de Informações (Dorking & Search Engines)
Analisando as pistas do enunciado:
- **Evento:** Protesto das panelas (*Kitchenware Revolution* / *Casserole Movement*), renúncia do Primeiro-Ministro em menos de 48 horas.
- **Vazamento:** Maior vazamento financeiro (11,5 milhões de documentos / 200.000 offshore) -> **Panama Papers (2016)**.
- **País:** Islândia.

Para validar os fatos e buscar os dados específicos, utilizei dorks nos buscadores (Google e DuckDuckGo):

```text
"Iceland" "Prime Minister" "Panama Papers" "renounced" "wife"
```

### 2. Análise dos Resultados
A pesquisa confirmou que o político em questão era **Sigmundur Davíð Gunnlaugsson**, ex-Primeiro-Ministro da Islândia.

Cruzando as informações com a base de dados do **ICIJ (Offshore Leaks Database)** e matérias jornalísticas do *The Guardian* e *BBC*:
- **Empresa Offshore:** `Wintris Inc.` (registrada nas Ilhas Virgens Britânicas).
- **Nome da Esposa:** `Anna Sigurlaug Pálsdóttir`.
- **Período de Vinculação:** Fundada no final de **2007**. Ele vendeu sua parte de 50% para a esposa por $1 em **31 de dezembro de 2009**.

---

## 🎯 Solução & Formatação da Flag

Durante a submissão, o maior desafio foi adequar o formato da string exata exigida pelo desafio (ex: maiúsculas/minúsculas ou separadores por underline).

Após validar a sintaxe esperada do desafio, a flag final foi estruturada com os dados coletados.

### 🚩 Flag
`HTB{Wintris_Inc_Anna_Sigurlaug_Palsdottir_2007_2009}`

*(Nota: Substitua o texto acima no formato exato que a plataforma aceitou no seu envio).*

---

⚠️ **Aviso importante**  
Todo o material aqui contido é para fins educacionais. As técnicas de investigação OSINT documentadas visam o aprendizado em cenários autorizados e de fontes abertas.

🚀 **Como contribuir**  
1. Faça um fork do repositório  
2. Crie uma branch: `git checkout -b feat/nova-solucao`  
3. Adicione seu write-up seguindo o template  
4. Commit: `git commit -m "feat: add write-up para desafio Panama Papers"`  
5. Push: `git push origin feat/nova-solucao`  
6. Abra um Pull Request  

📬 **Contato**  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com)  
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com)  

Happy Hacking! 🎯💻