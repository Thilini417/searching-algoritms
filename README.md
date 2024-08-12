# searching-algoritms

“Here, we will learn about keyword search, semantic search, and how they work, as well as how hybrid search integrates these methods.”

Keyword Search

Keyword search is a fundamental method used to retrieve information based on exact matches of user-provided terms. These keywords, or search terms, are the words or phrases entered by users to find products, services, or general information on platforms like search engines and e-commerce websites. For instance, in a Google search for “generative AI,” “generative AI” is the keyword.

This search approach relies on lexical text matching, focusing on the literal text of the query. It evaluates documents based on the presence and frequency of the query term. While effective for straightforward queries, keyword search may struggle with more complex or nuanced questions. A common algorithm used for keyword search is BM25, which assesses the relevance of documents based on term frequency and document length.

Semantic Search

Semantic search moves beyond simple keyword matching to understand the meaning behind the search queries. It involves search algorithms that analyze the semantics of the text rather than just the keywords. This method enables searches based on the meaning of the query, improving the relevance of the results for complex queries.

Semantic search can be leveraged through two primary techniques:

Dense Retrieval: This approach uses text embeddings to search for documents similar to a query. Text embeddings convert words into vectors (lists of numbers), capturing the semantic meaning of the text in a lower-dimensional space. By comparing these vectors, dense retrieval can identify contextually relevant documents.
Reranking: After an initial retrieval of items, reranking reorders the results to enhance their relevance or quality. It assigns a relevance score to each item based on its likelihood of being a correct response to the query. Training models for reranking involves providing positive and negative query-response pairs to help the system learn which responses are more relevant.
Hybrid Search

Hybrid search combines both keyword-based (sparse) and semantic (dense) search methods. This integration is particularly useful for large-scale applications where both precision and contextual relevance are important.

In a hybrid search system:

Keyword Search quickly narrows down the pool of relevant documents from a large corpus.
Semantic Search (dense retrieval) is then applied within this subset to identify the most contextually relevant documents based on embeddings.
The process begins with indexing the data, which consists of text. The data is then processed by a dense embedding model that generates vector representations. These vectors capture the semantic meaning of the input data in a high-dimensional space, allowing for both precise and meaningful search results.
