# Viwiki-Spelling: A dataset for Vietnamese Spelling Correction

## Introduction

## Details
The dataset contains 107 documents derived from [Vietnamese Wikipedia](https://vi.wikipedia.org/wiki/Wikipedia).
The dataset is stored in JSON lines and each document contains following key-value pairs:
```bash
{
    "_id": "Unique id in the dataset",
    "text": "the document content",
    "current_id": "revision current id",
    "parent_id": "revision parent id",
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
