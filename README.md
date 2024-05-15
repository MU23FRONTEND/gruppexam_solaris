# Solaris Space App

## Introduktion
Hejsan alla blivande kodastronauter!

Nu ska ni få ge er ut på ett hejdundrande rymdäventyr där ni kommer att bygga er alldeles egna interaktiva rymdapplikation i React med TypeScript. Er uppgift? Att skapa en portal som tar oss med på en spännande resa genom vårt eget lilla hörn av rymden - vårt solsystem!

## Uppgiften
Ni kommer att få bygga och även delvis designa en webbapplikation som tar användaren ut på en fascinerande resa genom solsystemet. Er applikation kommer att fungera som ett slags rymdlexikon, där användaren kan utforska och lära sig mer om våra närmsta grannar i rymden - planeterna!

## Krav (detta MÅSTE uppfyllas för godkänt)
- Er applikation skall bestå av följande pages
    - HomePage
    - PlanetPage
    - FavoritePage
- Er applikation skall MINST bestå av följande komponenter (ni får lägga till fler):
    - PlanetNav
    - Planet
    - PlanetDetails
- Ni skall använda CLI för att installera externa bibliotek och dependencies
- Ni skall använda er av useState och useEffect
- Ni skall använda er av routing
- Ni skall strukturera upp er css i olika filer
- Ni skall strukturera era typer i en models-mapp
- Ni skall presentera namnet på den planet användaren hovrar över i navigationen
- Ni skall implementera funktionalitet för att användaren skall kunna favoritmarkera en planet
- Ni skall designa och implementera en sida där användarens favoritplaneter listas
- Er kod får INTE innehålla några *any*-typer

## Design-instruktioner
- Designen för HomePage SKALL se ut på ett liknande sätt som i [mitt exempel](./assets/home-page-template.png) Det är valfritt att ge sig på Saturnus ringar, men storleken på planeterna måste på ett någorlunda vis förhålla sig relativt till varandra i storlek.
- Designen för PlanetPage väljer ni att antingen implementera [exempel 1](./assets/planet-page-example1.png), [eller exempel 2](./assets/planet-page-example2.png). Vid val av exempel 1 så skall backgrunden anpassas beroende på vilken planet som läses in. Vid val av exempel 2 skall bilden [star-transparent.png](./assets/star-transparent.png) i *assets*-mappen användas likt exempelbilden. Oavsett vilket exempel ni väljer så skall även funktionalitet för att lägga till/ta bort från favoriter implementeras.
- Designen för FavoritePage är helt valfri, men det måste se bra ut!
- Applikationen skall vara responsiv, och se bra ut på alla skärmar över 1000px i bredd.

## API-instruktioner
Detta blir lite speciellt då det är första gången som ni behöver interagera med en backend/molnet för att kunna få er webbsida att rocka. Det första ni måste göra är ett POST anrop mot url:en nedan:

```
POST https://n5n3eiyjb0.execute-api.eu-north-1.amazonaws.com/keys
```

Responset från anropet kommer innehålla den API-nyckel ni behöver för att göra ert GET-anrop. När ni nu har er nyckel så skall den skickas med headern 'x-zocom' i er request. Anropet hittar ni nedan:

```typescript
axios.get('https://n5n3eiyjb0.execute-api.eu-north-1.amazonaws.com/bodies', {
        headers : { 'x-zocom' : <här stoppar ni in er nyckel> }
    }).then...
```

## Grupper
### Grupp 1
Johan, Adam, Youssef

### Grupp 2
Nasser, Gaukhar, Inotila

### Grupp 3
Oleg, Carl Johan, Philip C

### Grupp 4
Philip N, Mahmoud, Tobias

Om jag missat någon som är aktiv i klassen så får ni kontakta mig så stoppar jag in er i en grupp.

Innan ni börjar arbeta så vill jag att varje grupp sätter sig ner och svarar på följande frågor:
- När och hur ska vi arbeta?
- Hur skall vi kommunicera med varandra?
- Vad gör vi om någon är sjuk?
- Vad gör vi om någon inte är med och arbetar aktivt i gruppen?
- Vad gör vi om någon inte svarar på meddelanden?

## Inlämning
Inlämning sker på Azomo, där var och en i gruppen länkar till gruppens gemensamma Git-repo senast kl 23:59 söndagen den 26 maj.





