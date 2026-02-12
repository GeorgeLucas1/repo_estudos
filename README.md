##SQL
apenas um cantinho pra colocar  meus script sql 
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/9b17fc53-548a-4474-ba8d-d6e0afaa03f9" />


# JOINS — Explicação Abstrata

## Conceito

Imagine duas listas:

- **Lista A**: pessoas convidadas para uma festa  
- **Lista B**: pessoas que realmente apareceram  

Os tipos de JOIN representam formas diferentes de comparar essas duas listas.

---

## INNER

Só entra no INNER se o valor existir na A e na B ao mesmo tempo por exemplo.
Mostra apenas quem está nas duas listas.

Convidado **e** compareceu.

**Resumo:** interseção das listas.

---

## LEFT

Mostra todos da **Lista A** (convidados).

Se a pessoa não compareceu, apenas indica que não foi.

**Resumo:** tudo da esquerda.

---

## RIGHT

Mostra todos da **Lista B** (quem apareceu).

Se alguém apareceu sem convite, ainda assim aparece.

**Resumo:** tudo da direita.

---

## FULL

Mostra todos das duas listas.

Inclui:
- Convidados que não foram  
- Pessoas que foram sem convite  
- Quem estava nas duas  

**Resumo:** tudo de tudo.

---

## Resumo Mental Final

- **INNER** → quem bate dos dois lados  
- **LEFT** → tudo da esquerda  
- **RIGHT** → tudo da direita  
- **FULL** → tudo de ambos  






