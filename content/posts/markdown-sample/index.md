---
title: "Przykłady Markdown"
date: 2020-06-08T08:06:25+06:00
description: Przykłady renderowania Markdown
menu:
  sidebar:
    name: Przykład Markdown
    identifier: markdown
    weight: 30
author:
  name: Anna Utracka
  image: /images/author/1_face.jpg
math: true
---

To jest przykładowy post mający na celu przetestowanie następujących elementów:

- Innego autora postu.
- Spisu treści.
- Renderowania treści Markdown.
- Renderowania matematyki.
- Renderowania emoji.

---
# Renderowanie Składni Markdown

## Nagłówki

Poniższe elementy HTML `<h1>`—`<h6>` reprezentują sześć poziomów nagłówków sekcji. `<h1>` to najwyższy poziom sekcji, a `<h6>` to najniższy.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Akapit

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Cytaty blokowe

Element blockquote reprezentuje treść cytowaną z innego źródła, opcjonalnie z cytatem, który musi znajdować się w elemencie `footer` lub `cite`, oraz opcjonalnie ze zmianami w tekście, takimi jak adnotacje i skróty.

#### Cytat blokowy bez atrybucji

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Uwaga**, że można używać *składni Markdown* wewnątrz cytatu blokowego.

#### Cytat blokowy z atrybucją

> Nie komunikuj się poprzez współdzielenie pamięci, współdziel pamięć poprzez komunikację.</p>
> — <cite>Rob Pike[^1]</cite>


[^1]: Powyższy cytat pochodzi z [wykładu](https://www.youtube.com/watch?v=PAAkCSZUG1c) Roba Pike'a podczas Gopherfest, 18 listopada 2015 r.

## Tabele

Tabele nie są częścią podstawowej specyfikacji Markdown, ale Hugo obsługuje je od razu po instalacji.

   | Imię  | Wiek |
   | ----- | --- |
   | Bob   | 27  |
   | Alice | 23  |

#### Wbudowany Markdown w tabelach

| Wbudowany&nbsp;&nbsp;&nbsp; | Markdown&nbsp;&nbsp;&nbsp; | W&nbsp;&nbsp;&nbsp;                | Tabeli |
| ------------------------ | -------------------------- | ----------------------------------- | ------ |
| *kursywa*                | **pogrubienie**                   | ~~przekreślenie~~&nbsp;&nbsp;&nbsp; | `kod` |

## Bloki kodu

#### Blok kodu z odwrotnymi apostrofami

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```
#### Blok kodu wcięty czterema spacjami

    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Blok kodu z wewnętrznym shortcode Hugo do podświetlania składni
{{< highlight html >}}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## Typy list

#### Lista uporządkowana

1. Pierwszy element
2. Drugi element
3. Trzeci element

#### Lista nieuporządkowana

* Element listy
* Kolejny element
* I jeszcze jeden element

#### Lista zagnieżdżona

* Owoce
  * Jabłko
  * Pomarańcza
  * Banan
* Nabiał
  * Mleko
  * Ser

## Inne Elementy — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> to format obrazu bitmapowego.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Naciśnij <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd>, aby zakończyć sesję.

Większość <mark>salamander</mark> prowadzi nocny tryb życia i poluje na owady, robaki i inne małe stworzenia.

---

## Renderowanie Matematyki

{{< math.inline >}}
<p>
Matematyka w linii: \(\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…\)
</p>
{{</ math.inline >}}

Matematyka blokowa:
$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } 
$$

---

## Renderowanie Emoji

<p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>