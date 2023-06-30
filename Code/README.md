  
  # Internal Skill-based Analysis
  We provide a comprehensive range of 13 methods for skill restructuring, which are detailed below:
  
        Abbreviation       |          Skill       
    =========================================================================================================================
    change_context_antonym | recognizing the adjectives
    mask_comparative       | recognizing the comparison
    shuffle_sentence_words | Understanding of grammatical rules and vocabulary organization of sentences.
    shuffle_sentence_order | Understanding of the sequence of events in the context.
    mask_numerics          | perform numerical calculations
    mask_pronouns	       | Detecting and understanding all occurrences of demonstrative pronouns
    drop_causal_words	   | Detecting and understanding all causal relationship rather than focusing on causal words
    mask_conditional	   | Explicit hypothetical reasoning rather than focusing on hypothetical words,
    drop_logical_words	   | Explicit logical reasoning rather than focusing on logical words
    drop_question_except_interrogatives	| Understanding of the question rather than focusing on the interrogative word
    drop_except_most_similar_sentences  | Inferencing with the whole context word rather than focusing on similar sentences
    drop_function_words	   | Understand context rather than focus on function words
    drop_content_words     | Understand context rather than focus on content words

[Specific introduction in the internal-skill-based-analysis
]https://github.com/distantJing/InDepth-Eva-MRC/tree/main/Analysis%20Principles%20Document#internal-skill-based-analysis

  ## 1. Install Python API
  ```cmd
    conda create -n CognitionSkill python=3.6 
    conda activate CognitionSkill
    git clone https://github.com/distantJing/InDepth-Eva-MRC.git
    cd ./Code
    pip3 install -r requirements.txt
    pip3 install Skill-0.0.1-py3-none-any.whl
 ```
  ## 2 Dwonload corenlp
    [stanford-corenlp-latest](https://huggingface.co/stanfordnlp/CoreNLP/tree/main)
    unzip stanford-corenlp-latest.zip
  ## 3. Use Python API
  ```python
    # An illustrative example of utilizing the "change_context_antonym" method to construct a dataset is as follows:

    # param introduce
    # skill : Skill Abbreviation
    # savepath : New Dataset Save Path
    # dataset : Dataset Name
    # loadpath : Original Dataset Save Path
    # corenlp : corenlp Save Path 
    from Skill import skill
    skill.main(skill='change_context_antonym',savepath='./save',dataset='SQuAD',loadpath='dataset/squad.json',corenlp='stanford-corenlp-4.5.4')
```




