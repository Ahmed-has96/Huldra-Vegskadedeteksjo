# Huldra — Vegskadedeteksjon

**Bacheloroppgave · Karakter A · 2025 · i samarbeid med Triona AS**

> ⚠️ Dette repoet inneholder kun dokumentasjon av prosjektet. Kildekoden er utviklet for og eies av Triona AS, og er derfor ikke offentlig tilgjengelig.

## Mitt bidrag

Jeg hadde hovedansvar for frontend. Jeg bygde kartvisningen i React og OpenLayers og koblet den til teamets .NET-API. I kartet kan brukeren se både hvor en skade ligger og hvor alvorlig den er.

## Hva prosjektet løser

Norske veimyndigheter samler inn enorme mengder LiDAR-data og informasjon fra NVDB (Nasjonal vegdatabank), men det er tidkrevende å omsette dette til konkrete beslutninger om hvor vedlikehold trengs mest. Huldra bygger bro mellom rådata og beslutning: systemet prosesserer LiDAR- og NVDB-data fra målebiler, beregner en tilstandsgrad fra 1–5 for veidekket, og presenterer resultatet i et interaktivt, fargekodet kart.

## Hvordan det fungerer

1. **Datainnhenting** — LiDAR (LAS-filer) og NVDB-data fra målebiler leses inn
2. **Prosessering** — Et .NET REST API renser og analyserer datasettene
3. **Tilstandsberegning** — En algoritme beregner en tilstandsgrad (1–5) per vegstrekning
4. **Visualisering** — Resultatene eksponeres som GeoJSON og vises i et interaktivt kart bygget med React, TypeScript og OpenLayers

## Teknologier

| Del | Teknologi |
|---|---|
| Frontend | React, TypeScript, OpenLayers |
| Backend | C#/.NET, REST API |
| Dataformat | GeoJSON, LiDAR/LAS, NVDB |
| Dokumentasjon | Swagger |

## Resultat

Prosjektet ga et konkret, visuelt beslutningsgrunnlag for vedlikeholdsplanlegging, og ble vurdert til karakter A. Utviklet i samarbeid med Triona AS som ekstern oppdragsgiver.

---

[Se porteføljen](https://ahmed-has96.github.io/) · [Les offentlig C#-kode fra F1 Special Event](https://github.com/Ahmed-has96/F1SpecialEvent/blob/main/Webutvikling/F1SpecialEventAPI/Controllers/DriversController.cs)
