
# Rapport

**Skriv din rapport här!**

Först forkades ett projekt från GitHub. Därefter för att öppna upp projektet i Android Studio, 
valdes `File` > `New` > `Project from version control`. Där finns sitt egna github-konto
och där hämtades projektet.

## Add a layout of your choice, e.g. `LinearLayout` or `ConstraintLayout`

Valde designläget för en mer bekvämlighet. I `Design` läget är det enkelt att lägga till 
val av layout till `Designer - Component Tree` genom att bara dra önskade views. I detta fall 
valdes en `constraint layout`. 

## Add a `ImageView` widgets inside the layout

I designläget under `palett` och `common` valdes en `ImageView` genom att dra den till fönstret 
`Designer - Component Tree`. Här kommer då ett fönster upp kallat `Pick a Resourse`. I detta fönster
finns möjlighet att välja befintlig data av bilder eller så går det välja egenvald bild. Här valdes 
egenvald bild från datorn genom att välja `+` uppe i vänstra hörnet. Sedan valdes `Import Drawables`. 
Då kommer man till datorns egna bilder. Viktigt här är att välja en `png-fil`. 

Valde sedan `quality type` > `next`. Då hamnade bilden i katalogen `res` och mappen `drawable`. 
Valde där bilden för att importera. Den hamnar då i `Widget.app.main` och där markerar man bilden 
och trycker `OK`. I designläget ändrades sedan bilden till önskad storlek och plats genom att med 
markören "dra" i bilden till önskad storlek samt plats.

## Add a `TextView` widgets inside the layout

I designläget under `palett` och `common` valdes en `TextView` genom att dra den till fönstret 
`Designer - Component Tree`. I `activity_main.xml` filen skapas då en kod för detta objekt. 
Se nedan kod (Kod.1). 

Denna kod ändrades en del i för att lägga till hundens namn, "Charlie" samt ändrades koden så att 
texten fick storleken 32sp samt centrerades texten. Detta gjordes genom att skriva in ny kod i 
`activity_main.xml` filen. Därefter ändrades även fonten på namnet "Charlie". Detta gjordes däremot 
i `Design` läget i `Declared Attributes` > `fontFamily` > `gorditas_bold`. Båda sättet är möjliga 
och här testades båda sätten. Koden för detta syns i nedan kod (Kod.2) Även här i `Design`
läget ändrades bakgrundsfärgen under `All Attributes` > `background`. 

Kod som lades till: 

```
<TextView
android:id="@+id/textView5"
android:layout_width="wrap_content"
android:layout_height="wrap_content"
android:text="TextView"
app:layout_constraintEnd_toEndOf="parent"
app:layout_constraintStart_toStartOf="parent"
tools:layout_editor_absoluteY="718dp" />
```
Kod som ändrades: 

```
<TextView
android:id="@+id/textView5"
android:layout_width="183dp"
android:layout_height="43dp"
android:fontFamily="@font/gorditas_bold"
android:text="Charlie"
android:textAlignment="center"
android:textColor="#844502"
android:textSize="32sp"
app:layout_constraintEnd_toEndOf="parent"
app:layout_constraintHorizontal_bias="0.479"
app:layout_constraintStart_toStartOf="parent"
app:layout_constraintTop_toBottomOf="@+id/imageView9" />
```

## Add a `Button` widgets inside the layout
I designläget under `palett` och `common` valdes en `Button` genom att dra den till fönstret
`Designer - Component Tree`. Då kom en vit "knapp" med texten text upp på devicen. Denna knappens
layout ändrades sedan genom tillvalen som finns under `Attributes`. Texten ändrades till `BARK`samt 
fonten, textstorleken och färgen, även knappens färg ändrades. 

En ljudeffekt av en skällande hund lades till knappen. Detta skapades genom att skapa en ny mapp 
genom att högerklicka på `res` > `New` > `Android Resource Directory`. Döpte mappen till `raw` där 
sedan en mp3 fil av hundskall lades till. Sedan var det bara att lägga till kod i 
´MainActivity.java` filen för att få detta att fungera. 




## Följande grundsyn gäller dugga-svar:

- Ett kortfattat svar är att föredra. Svar som är längre än en sida text (skärmdumpar och programkod exkluderat) är onödigt långt.
- Svaret skall ha minst en snutt programkod.
- Svaret skall inkludera en kort övergripande förklarande text som redogör för vad respektive snutt programkod gör eller som svarar på annan teorifråga.
- Svaret skall ha minst en skärmdump. Skärmdumpar skall illustrera exekvering av relevant programkod. Eventuell text i skärmdumpar måste vara läsbar.
- I de fall detta efterfrågas, dela upp delar av ditt svar i för- och nackdelar. Dina för- respektive nackdelar skall vara i form av punktlistor med kortare stycken (3-4 meningar).

Programkod ska se ut som exemplet nedan. Koden måste vara korrekt indenterad då den blir lättare att läsa vilket gör det lättare att hitta syntaktiska fel.

```
function errorCallback(error) {
    switch(error.code) {
        case error.PERMISSION_DENIED:
            // Geolocation API stöds inte, gör något
            break;
        case error.POSITION_UNAVAILABLE:
            // Misslyckat positionsanrop, gör något
            break;
        case error.UNKNOWN_ERROR:
            // Okänt fel, gör något
            break;
    }
}
```

Bilder läggs i samma mapp som markdown-filen.

![](android.png)

Läs gärna:

- Boulos, M.N.K., Warren, J., Gong, J. & Yue, P. (2010) Web GIS in practice VIII: HTML5 and the canvas element for interactive online mapping. International journal of health geographics 9, 14. Shin, Y. &
- Wunsche, B.C. (2013) A smartphone-based golf simulation exercise game for supporting arthritis patients. 2013 28th International Conference of Image and Vision Computing New Zealand (IVCNZ), IEEE, pp. 459–464.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A. (2012) Experimentation in Software Engineering, Berlin, Heidelberg: Springer Berlin Heidelberg.
