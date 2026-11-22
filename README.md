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
