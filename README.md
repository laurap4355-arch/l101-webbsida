# Moment 1: L101 Website

## Beskrivning

Detta är en webbplats som skapades i Laboration 1.

Webbplatsen handlar om att jag presentera mig själv, mina intressen och hobbyer.
Här presenteras information, bilder och innehåll som hör till mina hobbyer.

## Teknik

Webbplatsen är skapad med:

- HTML ( Används för att skapa sidans struktur)
- Git (Används för att spara olika kod version)
- GitHub (Lagring av kod online och projektdelning)

## Publicerade versioner

- [GitHub Pages](https://laurap4355-arch.github.io/l101-webbsida/)
- [Netlify] (https://lustrous-peony-8fed5f.netlify.app)

## Git-frågor

### Vad är skillnaden mellan git add och git commit?

`git add` väljer vilka ändringar som ska förberedas för commit.

`git commit` sparar de valda ändringarna som en ny version i Git.

Exempel:

```bash
git add .
git commit -m "Add new content"
```

### Varför använder man branches istället för att arbeta direkt i `main`?

Man använder branches för att kunna utveckla och testa nya ändringar utan att påverka huvudbranchen `main`.

I detta projekt användes branchen `dev` för att lägga till en ny bild. Därefter mergades ändringen tillbaka till `main`.

### Vad händer rent praktiskt när man gör en merge?

När man gör en merge kombineras ändringarna från en branch med en annan branch.

I detta projekt mergades `dev` in i `main`. Det betyder att ändringarna som gjordes i `dev` blev en del av huvudversionen i `main`.

### Vad är skillnaden mellan att pusha till GitHub och att publicera på Netlify?

`git push` skickar commits och kod från den lokala datorn till GitHub.

Netlify publicerar webbplatsen så att andra kan besöka den på Internet.

När Netlify är kopplat till GitHub kan en ny `git push` automatiskt starta en ny publicering på Netlify.

### Hur exkluderar man en fil från versionshanteringen?

Man skriver filens namn i filen `.gitignore`.

I detta projekt används `.gitignore` för att ignorera macOS-filen:

```
.DS_Store
```
Då kommer `.DS_Store` inte att versionshanteras av Git.