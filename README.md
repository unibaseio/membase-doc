# membase-doc
docs for membase layer


## Decentralized Memory Management: Redefining the Memory Architecture of Intelligent Agents

In traditional intelligent agent architectures, memory and data are typically managed by centralized servers, which pose potential risks related to data security and privacy. In contrast, in a decentralized intelligent agent system, the memory of the agent is finely divided into two parts: Prompt Context and the RAG Database. This architecture not only enables flexible memory management for intelligent agents but also ensures the privacy and security of data through decentralized storage.

+ Prompt Context: Every interaction with a user is automatically recorded by the intelligent agent, capturing the context of the conversation to provide more accurate and coherent responses in future interactions. Decentralized storage and management ensure that each user's contextual data is securely and privately stored, mitigating the risks of data misuse that are often found in traditional systems.

+ RAG Database: The RAG (Retrieval-Augmented Generation) database plays a central role in knowledge management. The intelligent agent utilizes this database to access real-time, updated knowledge in order to provide users with more accurate and in-depth responses. The decentralized storage not only enhances the efficiency of data access but also guarantees the high availability and reliability of the knowledge base through a distributed structure.

By decentralizing both the agent’s contextual memory and the knowledge management system, this architecture offers enhanced security, privacy, and resilience, making it a critical evolution in the development of intelligent agents.

## Components

Membase supports dify, swarms, weaviate and chroma. 

### Agent Framework

+ dify

```shell
# clone membase branch
# - use WEAVIATE_ENDPOINT(52.76.75.134:8081)
# - use HUB_ENDPOINT(http://54.151.130.2:8080)
> git clone -b membase https://github.com/unibaseio/dify.git
> cd dify/docker-compose
> docker compose up -d --build
```

+ swarms

```shell
# use HUB_ENDPOINT(http://54.151.130.2:8080)
> git clone -b membase https://github.com/unibaseio/swarms.git
> pip install -e .
```

### Vector Database

+ weaviate

```shell
#use HUB_ENDPOINT(http://54.151.130.2:8080)
> git clone -b membase https://github.com/unibaseio/weaviate.git
> cd weaviate/docker-compose 
> docker compose up -d --build
```

+ chroma

```shell
#use HUB_ENDPOINT(http://54.151.130.2:8080)
> git clone -b membase https://github.com/unibaseio/chroma.git
> pip install -e .
```