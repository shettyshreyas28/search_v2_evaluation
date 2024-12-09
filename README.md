# Search V2 Evaluation Suite

Utilities to run evaluation on search v2 results

Wrapper around the openai_batch_api repo to allow for users to run evals on search results

## Steps
* Clone the [openai_batch_pi](https://github.com/shettyshreyas28/openai_batch_api) repo 
* Follow instructions in the repo to setup .env and config.yaml in the folder 
* Create input file with *_id* column and *content* column (need to write function for content : f'search_question : {search_question} results: {str(results)}')
* Update prompt in the *config.yaml* file
* Run the batchapi calls and collate results
* Run ```python eval_summary.py``` to collate the summary of the results
