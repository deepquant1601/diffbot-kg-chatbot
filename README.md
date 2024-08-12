# News monitoring application and RAG chatbot

This project is designed to show an end-to-end pipeline for constructing knowledge graphs from news articles, analyzing them through various visualizations, and finally, allowing LLM to generate questions based on the information provided from the knowledge graph.

The project uses Neo4j, a graph database, to store the knowledge graph and Diffbot as the data provider. Diffbot offers various data integrations on its platform, such as:

* Latest or relevant news about a specific topic or company
* Extracting graph information from text
* Enriching organization or personal information

Lastly, the project uses OpenAI LLMs to provide a chat interface, which can answer questions based on the provided information from the knowledge graph.

## Setup

1. Set environment variables in `.env`. You can find the template in `.env.template`

2. Start the docker containers with

```
docker compose up 
```

3. Open you favorite browser on `localhost:3000`

## Contributions

Any contributions are welcomed through GitHub issues or pull requests.


Youtube presentation:
We're developing a GraphRAG system using Diffbot's APIs to construct reliable knowledge graphs, which are then stored in a Neo4j graph database for efficient querying and information retrieval.

0:00 intro
0:22 brief overview of graph rag and knowledge graphs
0:50 potential pitfalls of vector-based rag
1:29 graph rag research by microsoft
2:09 potential pitfalls of llms constructing knowledge graphs
2:20 brief intro of entity resolution
3:03 entity resolution problem with gpt-4
3:41 entity resolution handled by Diffbot
3:51 Graph RAG demo + article importer
4:37 web scraping without worrying about hallucinated sources
5:24 KG construction from news article
5:37 enrich the knowledge graph with Enhance API
5:57 final network graph
6:09 question answering (vector vs. vector+kg)
7:26 more examples (vector vs. vector+kg)
7:35 skip the outro and have fun with the repo!
7:52 attribution to Tomaž Bratanic and Anej Gorkič 
