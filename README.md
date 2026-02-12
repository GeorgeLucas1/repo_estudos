##SQL
apenas um cantinho pra colocar  meus script sql 
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/9b17fc53-548a-4474-ba8d-d6e0afaa03f9" />


# JOINS — Explicação Abstrata



<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/afe7c566-0a42-48e9-9e28-348e4bec83f3" />

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




# GROUP BY e HAVING — Explicação Simples

## Conceito Geral

Imagine uma lista de vendas:

| Pessoa  | Valor |
|----------|--------|
| Ana      | 100    |
| Ana      | 50     |
| Bruno    | 30     |
| Bruno    | 40     |
| Carlos   | 10     |

---

# GROUP BY

O `GROUP BY` serve para **agrupar dados semelhantes**.

Se agrupamos por **Pessoa**, juntamos todas as linhas da mesma pessoa.

Depois podemos aplicar um cálculo, como soma.

### Resultado agrupado (somando valores):

- Ana → 150  
- Bruno → 70  
- Carlos → 10  

Resumo:

`GROUP BY` cria grupos.

---

# HAVING

O `HAVING` serve para **filtrar os grupos depois que eles já foram criados**.

Exemplo:

Mostrar apenas quem vendeu mais que 100.

Após o agrupamento:

- Ana → 150  
- Bruno → 70  
- Carlos → 10  

Aplicando a regra:

Resultado:

- Ana → 150  

Resumo:

`HAVING` filtra grupos.

---

# Diferença Importante

- `WHERE` → filtra linhas antes de agrupar  
- `GROUP BY` → cria grupos  
- `HAVING` → filtra grupos depois de agrupados  

---

# Resumo Final

- GROUP BY → organiza em grupos  
- HAVING → aplica condição nos grupos  




