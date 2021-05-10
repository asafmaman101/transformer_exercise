Student 1:
* Name: Asaf Maman
* ID: 204209860
* Username: asafmaman

Now, for each log file that you need to submit, you will need to write its last 3 lines. For example, this is what we got for `baseline_gen.log`:
```txt
2021-04-24 17:20:46 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-04-24 17:20:46 | INFO | fairseq_cli.generate | Translated 7,283 sentences (165,025 tokens) in 18.5s (394.00 sentences/s, 8927.61 tokens/s)
Generate valid with beam=5: BLEU4 = 33.39, 69.1/42.8/28.5/19.4 (BP=0.934, ratio=0.937, syslen=138824, reflen=148229)
```

3 last lines from the baseline_train.log file: 
```txt
2021-05-06 02:21:47 | INFO | fairseq_cli.train | end of epoch 50 (average epoch stats below)
2021-05-06 02:21:47 | INFO | train | epoch 050 | loss 3.946 | nll_loss 2.516 | ppl 5.72 | wps 39816.9 | ups 3.82 | wpb 10419.8 | bsz 422.8 | num_updates 18950 | lr 0.000229718 | gnorm 0.614 | train_wall 54 | gb_free 7.8 | wall 5160
2021-05-06 02:21:47 | INFO | fairseq_cli.train | done training in 5159.4 seconds
```

3 last lines from the baseline_gen.log file: 
```txt
2021-05-06 08:00:45 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-06 08:00:45 | INFO | fairseq_cli.generate | Translated 7,283 sentences (167,248 tokens) in 22.5s (323.69 sentences/s, 7433.31 tokens/s)
Generate valid with beam=5: BLEU4 = 33.38, 68.4/42.2/28.0/19.0 (BP=0.947, ratio=0.948, syslen=140592, reflen=148229)
```

3 last lines from the baseline_mask.log file: 
```txt
2021-05-08 11:12:33 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-08 11:12:33 | INFO | fairseq_cli.generate | Translated 7,283 sentences (168,683 tokens) in 23.4s (311.56 sentences/s, 7216.18 tokens/s)
Generate valid with beam=5: BLEU4 = 32.19, 66.9/40.6/26.5/17.7 (BP=0.958, ratio=0.959, syslen=142104, reflen=148229)
```

25 last lines from the check_all_masking_options.log file: 
```txt
2021-05-08 12:11:48 | INFO | fairseq.tasks.translation | data-bin/iwslt14.tokenized.de-en valid de-en 7283 examples
2021-05-08 12:12:46 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-08 12:12:46 | INFO | fairseq_cli.generate | Translated 7,283 sentences (167,224 tokens) in 22.0s (330.81 sentences/s, 7595.78 tokens/s)
Generate valid with beam=5: BLEU4 = 33.09, 68.2/41.9/27.7/18.8 (BP=0.948, ratio=0.949, syslen=140688, reflen=148229)
table of score with masking enc-enc attention head
rows are transformer layer number and columns are head number
       0      1      2      3
0  33.34  33.35  33.16  33.13
1  33.24  33.36  33.23  33.24
2  33.28  32.76  32.25  33.32
3  33.19  33.02  29.94  33.29
table of score with masking enc-dec attention head
rows are transformer layer number and columns are head number
       0      1      2      3
0  33.32  33.17  17.92  32.92
1  33.02  33.07  33.03  33.23
2  33.09  33.44  32.74  32.60
3  32.19  32.56  32.29  32.50
table of score with masking dec-dec attention head
rows are transformer layer number and columns are head number
       0      1      2      3
0  33.26  33.26  33.30  33.29
1  33.39  33.11  33.26  33.51
2  33.42  33.45  32.48  33.26
3  33.26  33.43  33.18  33.09
```

3 last lines from the sandwich_train.log file: 
```txt
2021-05-10 12:55:35 | INFO | fairseq_cli.train | end of epoch 50 (average epoch stats below)
2021-05-10 12:55:35 | INFO | train | epoch 050 | loss 3.969 | nll_loss 2.542 | ppl 5.82 | wps 35564.3 | ups 3.41 | wpb 10419.8 | bsz 422.8 | num_updates 18950 | lr 0.000229718 | gnorm 0.622 | train_wall 58 | gb_free 7.8 | wall 5681
2021-05-10 12:55:35 | INFO | fairseq_cli.train | done training in 5681.0 seconds
```

3 last lines from the sandwich_gen.log file: 
```txt
2021-05-10 13:55:06 | INFO | fairseq_cli.generate | NOTE: hypothesis and token scores are output in base 2
2021-05-10 13:55:06 | INFO | fairseq_cli.generate | Translated 7,283 sentences (165,986 tokens) in 25.6s (284.03 sentences/s, 6473.34 tokens/s)
Generate valid with beam=5: BLEU4 = 33.25, 68.7/42.4/28.1/19.1 (BP=0.941, ratio=0.943, syslen=139726, reflen=148229)
```