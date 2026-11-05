# Maska

Svensk, mobilanpassad stickverkstad för barn och nybörjare. Buildless HTML, CSS och JavaScript i `dist/`.

- Fyra originalmotiv och lokal bilduppladdning (JPG/PNG/WebP/GIF, max 12 MB).
- Bilder skalas med bibehållet förhållande till en kvadratisk motivyta, samplas till maskor och kvantiseras till 2–5 garnfärger.
- Diagrammet har kolumn 1 till höger och rad 1 nederst. Varje cell motsvarar en maska. Kanten visas separat och ingår inte i diagrammet.
- Nybörjarteknik: enfärgad slätstickad ruta med rätstickad kant; motivet broderas efteråt med maskstygn.
- 3 kantmaskor per sida och 4 kantvarv uppe/nere. Udda inre varv stickas räta; jämna stickas 3 räta, N aviga, 3 räta.
- Beräknade mått från angiven stickfasthet är ungefärliga eftersom rätstickad kant har annan varvhöjd.
- Varvräknare, radbeskrivning för broderiet, lokal projektsparning, PNG-export och utskrift till PDF.

Ingen AI-tjänst eller serverbehandling används. Appen skapar motivdiagram och en fast, beräknad stickbeskrivning; den återskapar inte plaggs konstruktion från fotografier. Bilder lämnar inte enheten. Google Fonts används för typsnitten, med lokala systemtypsnitt som reserv.

## Validering

JavaScript syntaxkontroll. I webbläsare: färdigt motiv → beskrivning, varvräknare, spara → ladda om → återställ projekt, faktisk lokal PNG-uppladdning → nytt motiv och beskrivning. Teknikreferens: Purl Soho Duplicate Stitch (länk i hjälpen).

## Vercel

Statisk webbapp utan installations- eller byggsteg. `vercel.json` publicerar innehållet i `dist/`. Anslut GitHub-arkivet till Vercel med produktionsgrenen `main`.
