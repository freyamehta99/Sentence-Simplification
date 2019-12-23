#Sentence Simplification
This project aims to identify english sentences with more than two clauses and mark the clause boundaries. Additionally, breaking the complex/compound sentences into multiple simple sentences incorporating non-destructive simplification.
Following a rule-based method for this purpose, we primarily use constituency-based parse tree.

##HOW TO RUN
Run stanford parser:
```bash
java -mx4g -cp "*" edu.stanford.nlp.pipeline.StanfordCoreNLPServer -annotators "tokenize,ssplit,pos,lemma,parse,sentiment" -port 9000 -timeout 30000

python3 sent_to_clauses.py
```

##Authors: 
Freya Mehta(20171184) & Aamir Farhan(20161078)