---
tags:
  - Statistics/Models
---

1. Get text data
2. Decide if on character level or word level
3. Create an encoder/decoder to jump between string and numbers
4. Tokenize with encoder
5. Create train/test split
6. Pick block_size (what is the largest input size)
	1. Get the model used to receiving varying input to one output
	2. Could vary ranging from 1 to 8 inputs
7. Pick batch_size (how many inputs to train in parallel)
8. Input into the model will be a matrix where each row is a input vector. # rows = batch number
9. Create embedding, basically index -> One hot encoded vector
10. 