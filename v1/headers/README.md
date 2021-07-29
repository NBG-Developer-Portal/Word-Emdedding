#### Welcome to the Word Embedding API.

------------------------------------------------------------------------------------------
### The API
Start integrating your application with our Word Embedding API and give your client the options to:
* calculate closest of a word
* calculate distance between two words based on the trained word embedding model (Cosine similarity)


**Calculate closest of a word:**

Request:
  ```
  GET 'https://apis.nbg.gr/sandbox/word.embedding/headers/v1/words/closest?word=μικρότερη&num=10'
```
Response:
```
[
    {
        "word": "ίση",
        "distance": 0.31070899986498357
    },
    {
        "word": "όχι",
        "distance": 0.2421195967896132
    },
    {
        "word": "μέγιστη",
        "distance": 0.22128584618273286
    },
    {
        "word": "μηνών",
        "distance": 0.21824253573548197
    },
    {
        "word": "μηνιαία",
        "distance": 0.20402979844979469
    },
    {
        "word": "δέκα",
        "distance": 0.20319240773064454
    },
    {
        "word": "τριάντα",
        "distance": 0.1951317392615245
    },
    {
        "word": "θερμοκρασία",
        "distance": 0.19056630757567367
    },
    {
        "word": "μεγαλύτερο",
        "distance": 0.1880414347626946
    },
    {
        "word": "δεκαπέντε",
        "distance": 0.18796420721698445
    }
]
```



**Calculate distance between two words based on the trained word embedding model (Cosine similarity):**

Request:
```
GET 'https://apis.nbg.gr/sandbox/word.embedding/headers/v1/words/distance?word1=μικρότερη&word2=μέγιστη'
```
Response:
```
{
    "distance": 0.22128584618273286
}
```
