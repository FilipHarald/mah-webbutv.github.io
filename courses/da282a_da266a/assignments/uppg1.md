---
title: Inlämningsuppgift 1
code: da282a_da266a
---

# Inlämningsuppgift 1

Betyg: U/G

## Syfte

Syftet med den första inlämningen är att bekanta sig med både sin programmeringsmiljö (textredigare, terminal/kommandotolk, osv.) samt med grundläggande programmering. I det här fallet handlar det om att kunna spara data av olika typer (siffror och text) i variabler, för att sedan använda dessa för olika ändamål (t.ex. jämförelser eller uträkningar). Det handlar även om att skapa kod som är återanvändbar och dynamisk - funktioner, ett kärnkoncept inom programmering och något du kommer att stöta på i samtliga inlämningar.

Inför denna uppgift rekommenderas du starkt att läsa kapitel 1, 2, 3, 5 och 6 i boken _Think Python_ (gör gärna övningarna också).

Gå gärna även igenom "[kom igång](/courses/da282a_da266a/material/getting_started.html)".

## Uppgiften

Denna uppgift är indelad i mindre deluppgifter. Du rekommenderas att försöka hålla dig till den ordning som presenteras, då svårighetsgraden ökar för varje deluppgift. Uppgifterna kan lösas på många olika vis, det finns alltså inte alltid **ett** korrekt svar utan ibland kan det finnas ett flertal vägar för att nå rätt resultat. När du söker information via webben efter lösningar eller hjälp på vägen så rekommenderas du starkt att oavsett vad du hittar försöka förstå hur det fungerar. Experimentera och utforska gärna koden med Pythontolken.

**Tips:** Försök att skriva din Pythonkod på engelska, delvis för att det är en bra övning språkmässigt men framförallt så slipper du eventuella problem som kan uppstå med bokstäverna ÅÄÖ - om du inte stöter på dessa problem kan du bortse från detta tips.

**Glöm inte att läsa igenom kravspecifikationen innan du börjar, så du inte missar någonting eller får komplettera på grund av slarvfel.** 

Observera att i Pythonversion `3.x` sker utskrifter med `print(1)`, i Pythonversion `2.x` sker utskrifter med `print 1` - notera avsaknaden av parenteser
{: .info}

### Uppgift 1

Utifrån kodexemplet nedan ska du färdigställa samtliga utskrifter. Alla utskrifter ska ge värdet `True` och du får endast använda följande operatorer **en** gång var: `<`, `>`, `<=`, `==`, `!=`.

``` py
# Fyll i de operatorer som saknas
print(5 * 2   12)
print(55   22)
print(16 / 4   4)
print(8 + 2   128)
print(32 * 8   255)
```

### Uppgift 2

Ta reda på hur du kan få fram längden på en sträng (dvs. antal bokstäver i namnet nedan) och färdigställ exemplet nedan.

``` py
# The name
name = "Sherlock Holmes"
# Number of characters
num_of_chars = # ?
# Print the number of characters
print(num_of_chars)
```

### Uppgift 3

Tanken med uppgift 3 är att du ska slå ihop alla variabler (eng. _concatenate_). Vissa måste konverteras till strängar (eng. _string_) i variabeln `all_parts` som sedan skrivs ut.

``` py
part_1 = "The area of a Triangle with a width of "
part_2 = 12
part_3 = " and a height of "
part_4 = 8
part_5 = " is: "
# Calculate the area with the variables part_2
# and part_4 (the area is: height * width / 2)
part_6 = # ?

all_parts = # ?
print(all_parts)
```

### Uppgift 4

I uppgift 4 (två delar) ska du utföra något som kallas för _string slicing_, vilket innebär att vi skär av en bit från en sträng (text). För att göra detta kan du studera exemplet nedan och sedan gå vidare med de strängar du ska arbeta med.

#### Del 1

**Exempel**

``` py
# Example string
greeting = "Hello World!"
# Get a slice of the string
print(greeting[2:]) # => 'llo World!'
print(greeting[:2]) # => 'He'
print(greeting[:-2]) # => 'Hello Worl'
print(greeting[-2:]) # => 'd!'
print(greeting[2:-2]) # => 'llo Worl'
```

**Strängarna**

Tips: spara orginalsträngen (t.ex. "Tisdag" i en egen variabel likt exemplet ovan).

1. Skriv ut `"Tis"` av `"Tisdag"`
2. Skriv ut `"burgare"` av `"Hamburgare"`
3. Skriv ut `"be back"` av `"I'll be back"` 

#### Del 2

Fortsättningsvis ska du även arbeta med att konvertera från små till stora bokstäver och tvärtom. Detta kan göras på följande vis:

**Exempel**

``` py
# Example string
greeting = "Hello World!"
# Uppercase
print(greeting[:2].upper()) # => 'HE'
# Lowercase
print(greeting[:-2].lower()) # => 'hello worl'
```

**Strängarna**

1. Skriv ut `"LEARNING"` av `"It's Learning"`
2. Skriv ut `"good parts"` av `"Python: The Good Parts"`


### Uppgift 5

Skapa funktionen `calculate_triangle_area` som tar emot höjd och bredd och returnerar arean baserat på dessa. Ta en titt på exemplet nedan för att se hur vi hade kunnat använda oss av denna funktion.

``` py
# Print the area
print(calculate_triangle_area(12, 8)) # => 48

# Store the height and width in variables
# then calculate the area and finally print it
width = 12
height = 8
area = calculate_triangle_area(width, height)
print(area)
```

### Uppgift 6

I uppgift 5 ska du skapa två funktioner: `max` och `min`. Dessa ska ge tillbaka det största respektive minsta värdet av två siffror. För att förtydliga hur dessa används kan du ta en titt på exemplena nedan.

``` py
# Max
print(max(12, 17)) # => 17
print(max(15, 15)) # => 15
print(max(20, 3)) # => 20

# Min
print(min(12, 17)) # => 12
print(min(15, 15)) # => 15
print(min(20, 3)) # => 3
```

### Uppgift 7

Skapa en funktion som kontrollerar om en siffra är jämn, dvs. delbar med 2. Döp denna till `isEven`. Funktionen ska returnera `True` om siffran är jämn, annars `False`. Ta en titt på exemplet nedan för att se hur den kan användas.

``` py
print(isEven(10)) # => True
print(isEven(17)) # => False
```

Tips: Du kan använda dig av modulus-operatorn `%` för att kontrollera om någonting är jämnt, dvs. "om siffran - modulus - är det samma som 0".

## Kravspecifikation

* Placera alla uppgifter i en och samma Pythonfil med namnet `assignment_1.py`
* Markera samtliga uppgifter med en kommentar innehållande uppgiftsnummret, dvs. `# Uppgift 1`
* Använd sunt förnuft och dokumentera din Pythonkod med kommentarer där det kan anses vara lämpligt, t.ex. beskrivning av hur en funktion fungerar och ska användas
* Din Pythonkod ska fungera, dvs. den får inte generera något felmeddelande
* Din Pythonkod ska ha logiska namn vad gäller variabler och funktioner, dvs. inte `a = 10` eller `def x():`
* Kontrollera att din Pythonkod inte innehåller kodexempel från uppgiftsbeskrivning eller gamla kommentarer

## Inlämning

**Glöm inte att kontrollera att du skickat med svar på alla uppgifter och att du följt kravspecifikationen.**

När du är färdig med din uppgift ska du ladda upp denna som en `.zip`-fil innehållande alla dina filer på It's Learning. Döp denna enligt formatet `inl1_lisa_a.zip`.

Lycka till!
