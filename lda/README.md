The file train_lda.py trains an LDA model based on the documents in the specified JSON file.

Example for the THF corpus:
``` bash
 qsub -v input_file=/scratch_gs/malie102/data/lda/thf/corpus_tokenized-2015-07-07.json,loading_method=extract_nouns,blacklist_file=/scratch_gs/malie102/data/lda/thf/thf_blacklist,passes=500,output_path=/scratch_gs/malie102/data/lda/thf/lda_15,k=15 train_lda_hilbert.job
 qsub -v input_file=/scratch_gs/malie102/data/lda/thf/corpus_tokenized-2015-07-07.json,loading_method=extract_nouns,blacklist_file=/scratch_gs/malie102/data/lda/thf/thf_blacklist,passes=500,output_path=/scratch_gs/malie102/data/lda/thf/lda_5,k=5 train_lda_hilbert.job
 qsub -v input_file=/scratch_gs/malie102/data/lda/thf/corpus_tokenized-2015-07-07.json,loading_method=extract_nouns,blacklist_file=/scratch_gs/malie102/data/lda/thf/thf_blacklist,passes=500,output_path=/scratch_gs/malie102/data/lda/thf/lda_10,k=10 train_lda_hilbert.job
 qsub -v input_file=/scratch_gs/malie102/data/lda/thf/corpus_tokenized-2015-07-07.json,loading_method=extract_nouns,blacklist_file=/scratch_gs/malie102/data/lda/thf/thf_blacklist,passes=500,output_path=/scratch_gs/malie102/data/lda/thf/lda_20,k=20 train_lda_hilbert.job
 qsub -v input_file=/scratch_gs/malie102/data/lda/thf/corpus_tokenized-2015-07-07.json,loading_method=extract_nouns,blacklist_file=/scratch_gs/malie102/data/lda/thf/thf_blacklist,passes=500,output_path=/scratch_gs/malie102/data/lda/thf/lda_25,k=25 train_lda_hilbert.job
```