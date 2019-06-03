# Prefixed Headings in GitHub Flavored Markdown

[Outline headings with a decimal or alphanumeric prefix scheme](https://en.wikipedia.org/wiki/Outline_(list)) are desirable. The [GFM Spec](https://github.github.com/gfm) itself uses a decimal scheme. However, GFM does not do automatically numbered headings in plain Markdown.

## Decimal prefixes for Outline Headings

Auomatically numbered decimal outlines do not appear to be possible in GFM in any way.  If you want decimal prefixes, it appears that you need to manually include and increment the numbers yourself in each outline heading.

## Alphanumeric prefixes for Outline Headings

To do automatically numbered headings, you need to mix HTML with plain Markdown.

Below, in four sections, are (1) plain markdown, (2) that plain markdown rendered, and the same with HTML (3 & 4).  The fourth section is followed by notes about the workaround mix.

----

**1. PLAIN MARKDOWN:**

```` Markdown
## Et quidem, inquit, vehementer errat;

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam his libris eum malo quam reliquo ornatu villae delectari. Quid est igitur, inquit, quod requiras?

### Quae quidem vel cum periculo est quaerenda vobis;

Sed fac ista esse non inportuna; Faceres tu quidem, Torquate, haec omnia; Qua tu etiam inprudens utebare non numquam. Atqui reperies, inquit, in hoc quidem pertinacem; Ecce aliud simile dissimile. Quid vero? Quid enim possumus hoc agere divinius? Negat enim summo bono afferre incrementum diem.

### Color egregius, integra valitudo, summa gratia, vita denique conferta voluptatum omnium varietate.

Consequens enim est et post oritur, ut dixi. Immo alio genere; Iam id ipsum absurdum, maximum malum neglegi. Bona autem corporis huic sunt, quod posterius posui, similiora. Ego vero volo in virtute vim esse quam maximam; Cave putes quicquam esse verius.

## Quare attende, quaeso.

Sed quot homines, tot sententiae; Stoicos roga. Quorum altera prosunt, nocent altera. Maximus dolor, inquit, brevis est. Sed haec omittamus;

````

----

**2. THAT PLAIN MARKDOWN, RENDERED:**

## Et quidem, inquit, vehementer errat;

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam his libris eum malo quam reliquo ornatu villae delectari. Quid est igitur, inquit, quod requiras?

### Quae quidem vel cum periculo est quaerenda vobis;

Sed fac ista esse non inportuna; Faceres tu quidem, Torquate, haec omnia; Qua tu etiam inprudens utebare non numquam. Atqui reperies, inquit, in hoc quidem pertinacem; Ecce aliud simile dissimile. Quid vero? Quid enim possumus hoc agere divinius? Negat enim summo bono afferre incrementum diem.

### Color egregius, integra valitudo, summa gratia, vita denique conferta voluptatum omnium varietate.

Consequens enim est et post oritur, ut dixi. Immo alio genere; Iam id ipsum absurdum, maximum malum neglegi. Bona autem corporis huic sunt, quod posterius posui, similiora. Ego vero volo in virtute vim esse quam maximam; Cave putes quicquam esse verius.

## Quare attende, quaeso.

Sed quot homines, tot sententiae; Stoicos roga. Quorum altera prosunt, nocent altera. Maximus dolor, inquit, brevis est. Sed haec omittamus;

----

**3. THAT SAME TEXT MIXED WITH HTML TO PRODUCE HEADINGS WITH AUTOMATIC ALPHNUMERIC PREFIXES:**

```` Markdown
<ol type="A">
<h2><li>Et quidem, inquit, vehementer errat;</li></h2>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam his libris eum malo quam reliquo ornatu villae delectari. Quid est igitur, inquit, quod requiras?

<ol type="1">
<h3><li>Quae quidem vel cum periculo est quaerenda vobis;</li></h3>

Sed fac ista esse non inportuna; Faceres tu quidem, Torquate, haec omnia; Qua tu etiam inprudens utebare non numquam. Atqui reperies, inquit, in hoc quidem pertinacem; Ecce aliud simile dissimile. Quid vero? Quid enim possumus hoc agere divinius? Negat enim summo bono afferre incrementum diem.

<h3><li>Color egregius, integra valitudo, summa gratia, vita denique conferta voluptatum omnium varietate.</li></h3>

Consequens enim est et post oritur, ut dixi. Immo alio genere; Iam id ipsum absurdum, maximum malum neglegi. Bona autem corporis huic sunt, quod posterius posui, similiora. Ego vero volo in virtute vim esse quam maximam; Cave putes quicquam esse verius.

<ol>
<li>Third Level Heading</li>
Third level text.

<ol>
<li>Fourth Level Heading</li>
Fourth level text. 

</ol>

</ol>

</ol>

<h2><li>Quare attende, quaeso.</li></h2>

Sed quot homines, tot sententiae; Stoicos roga. Quorum altera prosunt, nocent altera. Maximus dolor, inquit, brevis est. Sed haec omittamus;

</ol>

````


----
**4. THAT SAME TEXT MIXED WITH HTML, RENDERED:**

<ol type="A">
<h2><li>Et quidem, inquit, vehementer errat;</li></h2>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam his libris eum malo quam reliquo ornatu villae delectari. Quid est igitur, inquit, quod requiras?

<ol type="1">
<h3><li>Quae quidem vel cum periculo est quaerenda vobis;</li></h3>

Sed fac ista esse non inportuna; Faceres tu quidem, Torquate, haec omnia; Qua tu etiam inprudens utebare non numquam. Atqui reperies, inquit, in hoc quidem pertinacem; Ecce aliud simile dissimile. Quid vero? Quid enim possumus hoc agere divinius? Negat enim summo bono afferre incrementum diem.

<h3><li>Color egregius, integra valitudo, summa gratia, vita denique conferta voluptatum omnium varietate.</li></h3>

Consequens enim est et post oritur, ut dixi. Immo alio genere; Iam id ipsum absurdum, maximum malum neglegi. Bona autem corporis huic sunt, quod posterius posui, similiora. Ego vero volo in virtute vim esse quam maximam; Cave putes quicquam esse verius.

<ol>
<li>Third Level Heading</li>
Third level text.

<ol>
<li>Fourth Level Heading</li>
Fourth level text. 

</ol>

</ol>

</ol>

<h2><li>Quare attende, quaeso.</li></h2>

Sed quot homines, tot sententiae; Stoicos roga. Quorum altera prosunt, nocent altera. Maximus dolor, inquit, brevis est. Sed haec omittamus;

</ol>

----

**NOTES REGARDING THE WORKAROUND MIX WITH HTML:**

As you may have noticed, mix's first level in the outline is numbered with uppercase letters.  We expected that because of [the type attribute](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol) in the tag `<ol type="A">`.

However, the mix's second level in the outline has lowercase Roman numerals despite the tag `<ol type="1">`.  That is because [a GitHub stylesheet](https://github.githubassets.com/app/node_modules/@primer/css/base/typography-base.scss) has a `list-style-type` property that instructs the browser to render such a second-level `ol` with lowercase Roman numerals.  

GitHub CSS `list-style-type` property overrides by level:
1. None.  Whatever valid `ol type` you specify is what you will get:  "I", "A", "1", "i", or "a".
2. Lowercase roman numerals.
3. Lowercase letters.
4. Lowercase letters.
5. Lowercase letters.

Lowercase letters are used for every level from 3 onward.  The GitHub stylesheet instructs that any `ol` that is nested within two `ol` tags (or within any combination of two `ol` or `ul` tags) should be displayed as lowercase letters. :(
