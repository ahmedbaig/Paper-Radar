# paper-radar

Daily arXiv ingestion focused on geospatial AI and remote sensing, ranked by a model trained on my own labels, delivered as a short daily digest and a private podcast.

## Phases

1. **Ingest:** pull new papers daily from chosen arXiv categories into Postgres.
2. **Rank:** label papers (interested / not), train a ranker on those labels, improve it as labels accumulate.
3. **Digest:** a daily list of the top papers.
4. **Audio:** a language model scripts the top papers for listening, local text-to-speech voices them, and a private podcast feed delivers them (5 to 10 minute daily digest, optional weekly deep dive).

Reuses [memory-store](https://github.com/ahmedbaig/memory-store) for embeddings and search where it fits.
