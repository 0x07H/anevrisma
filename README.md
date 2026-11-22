# anevrisma
fixme


Κανόνες Outlook. Click `...` [Περισσότερες ενέργειες]

```
[...new Set(
  [...document.querySelectorAll('[aria-label*="κανόνας" i]')]
    .map(el => el.getAttribute('aria-label').split(':')[0])
)]

Array(4) [ "Σύμπτυξη κανόνας", "Επεξεργασία κανόνας", "Διαγραφή κανόνας", "Ανάπτυξη κανόνας" ]
```


Let $T$ be the translation function and $\oplus$ denote the concatenation of words with a space.

$$
\begin{aligned}
T(\text{Collapse}) &= \text{Σύμπτυξη}\\
T(\text{rule}) &= \text{κανόνας}
\end{aligned}
$$

If translation were a homomorphism with respect to concatenation, then:

$$
\forall x,y:\quad T(x\oplus y)=T(x)\oplus T(y)
$$

Therefore:

$$
T(\text{Collapse rule}) = \text{Σύμπτυξη κανόνας}
$$

However, the correct translation is:

$$
T(\text{Collapse rule}) = \text{Σύμπτυξη κανόνα}
$$

**Thus, translation is not a homomorphism with respect to word concatenation.**

$$
\boxed{
\exists x,y:\quad
T(x\oplus y)\neq T(x)\oplus T(y)
}
$$



How the turntables:
- § 4.1.10 Genitive https://aka.ms/greek-styleguide
  - https://learn.microsoft.com/en-us/globalization/reference/microsoft-style-guides
- Do not use composite strings that are built at runtime from concatenated phrases. Composite strings are difficult to localize because they often assume an English grammatical order that does not apply to all languages.
  - https://learn.microsoft.com/en-us/dotnet/core/extensions/best-practices-for-developing-world-ready-apps#localization-best-practices
- Declensions 
  - https://learn.microsoft.com/en-us/globalization/internationalization/concatenation#declensions
- Concatenation is never used to assemble messages or user interface labels. 
  - https://learn.microsoft.com/en-us/globalization/testing/internationalization-checklist#localizability
