# :bulb: KnowThyselves
A company-internal knowledge graph prototype I developed in 2023 in the context of the Workstream "Learning Organization" at DigitalService, together with Ilya Alexander Yacine.

It was accompanied by an internal repository containing some scripts I wrote to import triples into the knowledge graph from various sources.

After some months of working on it on the side, the project was abandoned.

See some screenshots [here](app-screenshots/list.md).

<figure style="text-align:center">
  <img title="Katy" src="https://user-images.githubusercontent.com/5141792/225292599-c8ae735f-10f9-42c3-89c2-267a1d60b790.png" width="400" alt="Katy">
  <figcaption style="text-align:center"><i>Katy</i></figcaption>
</figure>

## Tech stack

Find diagrams in `doc`.

## How to run the application

For a quick demo with some data (and various mockups for the demo-narrative) readily available, go back to tag [v0.1.0-demo](https://github.com/digitalservicebund/know-thyselves/releases/tag/v0.1.0-demo). The current state on `main` will not import demo-data upon startup.

### Backend

```sh
cd backend
./gradlew bootRun
```

Or as IntelliJ run configuration:

![](https://user-images.githubusercontent.com/5141792/226630200-34a24bd5-4d36-4803-b263-db247f42609e.png)

<!-- See which environment variables have to be set in `application.properties`. -->

### Frontend


```sh
cd frontend
npm install
npm start
```

<!-- Fill the values in `frontend/src/config.json`:
```json
{
    "SPARQL_ENDPOINT": ""
}
```-->

## Other

- `scripts/miro` detects a graph on Miro (sticky notes with labelled connection lines between them) and exports it to:
  - a TGF or Turtle file (commented out)
  - a SPARQL endpoint
