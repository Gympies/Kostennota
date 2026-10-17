## Stack

Frontend: React + TypeScript + Vite. Backend: FastAPI, Pydantic v2, SQLAlchemy 2, Python 3.14.

## Regels

1. **Contracten eerst:** elk request en elke response is een Pydantic-schema.
2. **Lagen:** routes (alleen HTTP) > services (regels en autorisatie) > models. Routes raken de database nooit rechtstreeks aan.
3. De huidige gebruiker komt uit `get_current_user`. Vertrouw nooit een school-id die de browser meestuurt; filter elke query op de geverifieerde school.
4. Geen geheimen in code. Instellingen via omgevingsvariabelen; `.env` staat in `.gitignore`.
5. Elke wijziging krijgt een test. Bij een bug: eerst een falende test.
6. Werk in kleine stappen en wijzig niets buiten de gevraagde stap. Stop na elke stap.
7. Geen echte persoonsgegevens in code, tests of voorbeelden: gebruik verzonnen data.

## Werkwijze

Leg eerst uit wat je gaat doen. Vraag bij twijfel of een ontbrekend gegeven om verduidelijking.
