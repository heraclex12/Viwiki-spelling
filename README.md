# Viwiki-Spelling: A test dataset for Vietnamese Spelling Correction

## Introduction
We introduce a first Vietnamese Spelling Correction dataset containing manual labeling mistakes and corresponding correct words.

## Details
The dataset contains 107 documents derived from [Vietnamese Wikipedia](https://vi.wikipedia.org/wiki/Wikipedia).
The dataset is stored in JSON lines and each document contains following key-value pairs:
```bash
{
    "_id": "Unique id in the dataset",
    "text": "the document content",
    "current_id": "revision current id",
    "parent_id": "revision previous id",
    "page_id": "viwiki id",
    "mistakes": [
                  {
                    "text": "mistake word 1",
                    "start_offset": "index in the document",
                    "suggest": ["correct word 1", "correct word 2", ...]
                  },
                  ...
                ]
}
```

## License
The dataset is under [Attribution 4.0 International (CC BY 4.0)](LICENSE)

## Cite
```
@InProceedings{10.1007/978-3-030-79457-6_46,
author="Tran, Hieu
and Dinh, Cuong V.
and Phan, Long
and Nguyen, Son T.",
editor="Fujita, Hamido
and Selamat, Ali
and Lin, Jerry Chun-Wei
and Ali, Moonis",
title="Hierarchical Transformer Encoders for Vietnamese Spelling Correction",
booktitle="Advances and Trends in Artificial Intelligence. Artificial Intelligence Practices",
year="2021",
publisher="Springer International Publishing",
address="Cham",
pages="547--556",
isbn="978-3-030-79457-6"
}

```
