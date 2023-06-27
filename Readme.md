# Podcast Summary + Questioning Example

Minimal example of a podcast summary and questioning system using Whisper for Podcast transcription and GPT 3.5-turbo for summarization and questioning. Additionally we use HyDe Embeddings as the Summary/Questions are in German and the source information is in English.


## Install:
(Jupyter kernel, FFMPEG and Python 3.10+ needed)
```bash
poetry install
```

## Usage:

* Download Podcast Episode and put in `podcast/Podcast.mp3` .
* Run `podcast_transcript_demo.ipynb` to generate the transcript and Question answering system.

## Examples:

### Podcast Summary

Summary of [this](https://www.youtube.com/watch?v=doupx8SAs5Y) podcast episode with Tim Feriss:

```
Tim Ferriss betont die Bedeutung des bewussten Zeitmanagements, der Auswahl der richtigen Aktivitäten und Menschen sowie der Fähigkeit, sich auf das Wesentliche zu konzentrieren, um ein erfülltes und erfolgreiches Leben zu führen. Er spricht auch über die Bedeutung von Deoptimierung und Pausen, um Unbehagen zu erleben und neue kreative Energien freizusetzen. 

Ferriss betont die Vorteile von Mentoren und die Bedeutung des Lernens von fast jedem. Er spricht auch über die Wichtigkeit der Aufmerksamkeitszuweisung und des Zeitmanagements, um sich auf wichtige Aktivitäten zu konzentrieren und Ablenkungen zu vermeiden. Ferriss erwähnt den Einfluss von sozialen Medien auf die Aufmerksamkeit und betont die Notwendigkeit, bewusst mit ihnen umzugehen. Insgesamt betont er die Bedeutung von Energie, Kreativität und der Verfolgung von Projekten, die uns Freude bereiten. Ferriss teilt auch persönliche Erfahrungen, wie seine eigene Suizidgedanken in der Vergangenheit, um anderen zu helfen und ihnen Mut zu machen, über ihre eigenen mentalen Herausforderungen zu sprechen. 

Darüber hinaus hat er auch über seine Erfahrungen mit sexuellem Missbrauch gesprochen und wie er sich entschieden hat, diese Erfahrungen öffentlich zu teilen, um anderen zu helfen und Hoffnung zu geben. Seine Offenheit hat bereits vielen Menschen geholfen und ermutigt andere, ihre eigenen Traumata anzusprechen. Ferriss identifiziert sich hauptsächlich als Experimentalist und Lehrer und betont die Bedeutung von Rollenidentität. 

Er erwähnt auch sein Interesse an Kunst und seine frühere Karriere als Illustrator. Er möchte seine Fähigkeiten in der visuellen Kunst weiterentwickeln und auch Animation ausprobieren. Darüber hinaus erwähnt er den Wunsch, irgendwann Vater zu werden und betont die Unterschiede zwischen dem Wunsch, Kinder zu haben, und dem Wunsch, ein guter Elternteil zu sein.
````


### Question Answering

```
> qa.run("Was sind Tim Feriss Erfahrungen im Bezug auf geistige Gesundheit?")

'Tim Ferriss hat sich intensiv mit dem Thema geistige Gesundheit auseinandergesetzt und ist ein Befürworter der Verwendung von psychedelischen Substanzen zur Behandlung von psychischen Erkrankungen wie Depressionen, Essstörungen und Sucht. Er hat mehrere Millionen Dollar für die Erforschung von psychedelischer Therapie gespendet und hat damit maßgeblich dazu beigetragen, dass dieses Feld von der Randwissenschaft zur etablierten Forschung mit Unterstützung durch Philanthropie und staatliche Fördermittel geworden ist. Tim Ferriss hat sich auch für verschiedene philanthropische Projekte engagiert und setzt sich aktiv für die Verbesserung der geistigen Gesundheit ein.'
````
