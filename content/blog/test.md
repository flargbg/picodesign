---
Title: The struggle is real
Date: 2024-11-14
Author: relaxing
Description: Från en simpel testsida blev detta ett litet tips & tricks för andra läsare. Här kan du läsa om hur jag formatterade mitt blog post.
Template: blog
---

Första bloggen (test)
=================================

## Strul med att få i gång

Steg 1
: Lite komplettering till dokumentation skulle jag nog säga. Det var inte helt lätt att fixa bloggen. Utan `Title` metan skapades ingen länk. Aja det är fixat, nu ska vi få in rackaren i menyn.

Steg 2
: Verkar som att allting behöver en `Title` tag för att fungera. Är nöjd och glad. Länken finns med i huvudmenyn. Nästa steg blir att klura ut hur vi ska få in den i en möjlig framtida sidmeny.

Steg 3
: Ville självklart ha med en bild, menar vad för blogpost är där utan bild. Det var inte lätt, snarare sagt inte möjligt kanske? Vet inte, googlat en massa och läst om YAML headers. Det fanns ingen `key` som hanterade sådant enligt min förståelse. Då lekte problemlösningshjärnan runt lite och kom på att det är inte viktigt för mig att nämna `Author`, använder metan istället för bilden på bloggen. Därefter byggde jag upp länken på följande vis `src="{{ ASSETS_URL }}/img/{{ page.author }}.png"`. Lite komplicerat men det viktiga är att den uppfyller sitt syfte, dock inte enligt Pico säkerligen.