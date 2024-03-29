# Randomized Motif Discovery Algorithm
----------------------------------------

We introduced "Random Restart" in the algorithm, as the complexity of the algorithm is exponential and it would end up taking a huge time for generating result. In case of being stuck at a local maxima, the random restarts checks for any improvement, if none, it restarts the process from the beginning and thus the stuck at local maxima problem is solved. Also, at each iteration, each generated motif is checked using entropy of the found best result for improvement. Upon a lesser entropy improvement the result is updated.

## Sample run on hm03

- **Number of sequences available:** 10
- **Length of k-mer:** 10
- **Maximum iterations:** 1000
- **Restart threshold:** 10

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | GATAAAGGGA    | 1500            |
| Sequence 2 | GACACAGGGA    | 1500            |
| Sequence 3 | GACACAGGGA    | 1500            |
| Sequence 4 | GAAACAGGGA    | 1500            |
| Sequence 5 | GACACAGGAA    | 1500            |
| Sequence 6 | GAAACTGGGA    | 1500            |
| Sequence 7 | GACACAGGAA    | 1500            |
| Sequence 8 | GAAACAGGAC    | 1500            |
| Sequence 9 | GGCACAGGGA    | 1500            |
| Sequence 10| GAAAAGGGGA    | 1500            |

**Entropy of the generated motifs:** 1.3103084497384816


- **Number of sequences available:** 10
- **Length of k-mer:** 5
- **Maximum iterations:** 1000
- **Restart threshold:** 10

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TTTGC         | 1500            |
| Sequence 2 | TTTGC         | 1500            |
| Sequence 3 | TTTGC         | 1500            |
| Sequence 4 | TTTGC         | 1500            |
| Sequence 5 | TTTGC         | 1500            |
| Sequence 6 | TTTGC         | 1500            |
| Sequence 7 | TTTGC         | 1500            |
| Sequence 8 | TTTGC         | 1500            |
| Sequence 9 | TTTGC         | 1500            |
| Sequence 10| TTTGC         | 1500            |

**Entropy of the generated motifs:** 1.0892300788425848
This is the lowest possible entropy for 10 sequences. We would not get entropy zero for the reason that we are using Laplace's Rule of Succession which would increase the overall entropy.


- **Number of sequences available:** 10
- **Length of k-mer:** 15
- **Maximum iterations:** 1000
- **Restart threshold:** 10

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | GAGAAGAGAAAATGA | 1500            |
| Sequence 2 | GAAAAGAGAAAGTGA | 1500            |
| Sequence 3 | GAGAGGAGGAAGAGA | 1500            |
| Sequence 4 | GAATAGTAAAAAAGA | 1500            |
| Sequence 5 | CCAAAATGGAAAAGA | 1500            |
| Sequence 6 | GAAAACACAAAAAGA | 1500            |
| Sequence 7 | AAAAACTCAAAATGA | 1500            |
| Sequence 8 | GTAAAGCTGAAGAGG | 1500            |
| Sequence 9 | AAAAAAAAAAAAAGA | 1500            |
| Sequence 10| CTAAAGGTGAAAAGG | 1500            |

**Entropy of the generated motifs:** 1.479303304549106

## Sample run on yst04r

- **Number of sequences available:** 7
- **Length of k-mer:** 10
- **Maximum iterations:** 1000
- **Restart threshold:** 10

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TTTTTTTCTT    | 1000            |
| Sequence 2 | TATTTTTCTT    | 1000            |
| Sequence 3 | TATTTTTTTT    | 1000            |
| Sequence 4 | TTTTTTTCTT    | 1000            |
| Sequence 5 | TATTTTACTT    | 1000            |
| Sequence 6 | TATTTTTCTT    | 1000            |
| Sequence 7 | TATTTTTTTT    | 1000            |

**Entropy of the generated motifs:** 1.366878805297442


- **Number of sequences available:** 7
- **Length of k-mer:** 5
- **Maximum iterations:** 1000
- **Restart threshold:** 10

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TTAAT         | 1000            |
| Sequence 2 | TTAAT         | 1000            |
| Sequence 3 | TTAAT         | 1000            |
| Sequence 4 | TTAAT         | 1000            |
| Sequence 5 | TTAAT         | 1000            |
| Sequence 6 | TTAAT         | 1000            |
| Sequence 7 | TTAAT         | 1000            |

**Entropy of the generated motifs:** 1.2776134368191154
This is the lowest possible entropy for 7 sequences. We would not get entropy zero for the reason that we are using Laplace's Rule of Succession which would increase the overall entropy.


- **Number of sequences available:** 7
- **Length of k-mer:** 15
- **Maximum iterations:** 1000
- **Restart threshold:** 10

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TTTTTTTTTCTTTCC | 1000            |
| Sequence 2 | AATATTTTTCTTTTT | 1000            |
| Sequence 3 | TATTATTTTTATATT | 1000            |
| Sequence 4 | TTTTTTTTTCTTTTC | 1000            |
| Sequence 5 | TACTTCTTTCTTGTA | 1000            |
| Sequence 6 | TTTATTTTTCTTTTC | 1000            |
| Sequence 7 | TATTTTTTTTTGTT  | 1000            |

**Entropy of the generated motifs:** 1.5054170720285864

## Sample run on yst08r

- **Number of sequences available:** 11
- **Length of k-mer:** 10
- **Maximum iterations:** 1000
- **Restart threshold:** 10  # For random restart

| Sequence   | Motif       | Sequence length |
|------------|-------------|-----------------|
| Sequence 1 | TCTTTTGTTT  | 1000            |
| Sequence 2 | TTTTTTTTCT  | 1000            |
| Sequence 3 | TTTTTTTTTT  | 1000            |
| Sequence 4 | TTTTTTTTTT  | 1000            |
| Sequence 5 | TTTTTTGTTT  | 1000            |
| Sequence 6 | TTTTTTATTT  | 1000            |
| Sequence 7 | TTTTTTTTTT  | 1000            |
| Sequence 8 | TTTTTTTTTT  | 1000            |
| Sequence 9 | TTTTTTCTAT  | 1000            |
| Sequence 10| TTTTTTCTTT  | 1000            |
| Sequence 11| TTTTTTGTTT  | 1000            |

**Entropy of the generated motifs:** 1.1823936534688424

- **Number of sequences available:** 11
- **Length of k-mer:** 5
- **Maximum iterations:** 1000
- **Restart threshold:** 10  # For random restart

| Sequence   | Motif       | Sequence length |
|------------|-------------|-----------------|
| Sequence 1 | AGAAA       | 1000            |
| Sequence 2 | AGAAA       | 1000            |
| Sequence 3 | AGAAA       | 1000            |
| Sequence 4 | AGAAA       | 1000            |
| Sequence 5 | AGAAA       | 1000            |
| Sequence 6 | AGAAA       | 1000            |
| Sequence 7 | AGAAA       | 1000            |
| Sequence 8 | AGAAA       | 1000            |
| Sequence 9 | AGAAA       | 1000            |
| Sequence 10| AGAAA       | 1000            |
| Sequence 11| AGAAA       | 1000            |

**Entropy of the generated motifs:** 1.0389205950315936
This is the lowest possible entropy for 11 sequences. We would not get entropy zero for the reason that we are using Laplace's Rule of Succession which would increase the overall entropy.

- **Number of sequences available:** 11
- **Length of k-mer:** 15
- **Maximum iterations:** 1000
- **Restart threshold:** 10  # For random restart

| Sequence   | Motif           | Sequence length |
|------------|-----------------|-----------------|
| Sequence 1 | TTTATTTTACTTCTT | 1000            |
| Sequence 2 | TTTTTTTTCTCCATT | 1000            |
| Sequence 3 | TTTTTTTAGCTCATT | 1000            |
| Sequence 4 | TTTTTATTCTTAACT | 1000            |
| Sequence 5 | TTCTTTTTTTTAATT | 1000            |
| Sequence 6 | ATTCTATTTTTTATT | 1000            |
| Sequence 7 | TTTTTTTTTTTGATT | 1000            |
| Sequence 8 | TTTTTTTTTTCCATT | 1000            |
| Sequence 9 | TTGTGATGTTTTATC | 1000            |
| Sequence 10| TTTTTATTTTAGATT | 1000            |
| Sequence 11| TTTTTCTTTTTAATT | 1000            |

**Entropy of the generated motifs:** 1.3913574276603924


# Gibbs Sampling Algorithm
---------------------------

## Sample run on hm03

- **Number of sequences available:** 10
- **Length of k-mer:** 10
- **Number of iterations:** 10000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TGCTGATTGG    | 1500            |
| Sequence 2 | TGATGAGTGC    | 1500            |
| Sequence 3 | TGCTGATTGT    | 1500            |
| Sequence 4 | AGATGAGTCT    | 1500            |
| Sequence 5 | CGCTGATTCC    | 1500            |
| Sequence 6 | GGCTGAGTGG    | 1500            |
| Sequence 7 | TGGTGATTTT    | 1500            |
| Sequence 8 | AGCTGAGTCT    | 1500            |
| Sequence 9 | TGGTGAATGT    | 1500            |
| Sequence 10| TGCTGAGTCT    | 1500            |

**Entropy of the generated motifs:** 1.412808773081848


- **Number of sequences available:** 10
- **Length of k-mer:** 5
- **Number of iterations:** 1000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | AATGA         | 1500            |
| Sequence 2 | AATGA         | 1500            |
| Sequence 3 | AATGA         | 1500            |
| Sequence 4 | AATGA         | 1500            |
| Sequence 5 | AATGA         | 1500            |
| Sequence 6 | AATGA         | 1500            |
| Sequence 7 | AATGA         | 1500            |
| Sequence 8 | AATGC         | 1500            |
| Sequence 9 | AATGA         | 1500            |
| Sequence 10| AATGA         | 1500            |

**Entropy of the generated motifs:** 1.1297224625016797


- **Number of sequences available:** 10
- **Length of k-mer:** 15
- **Number of iterations:** 1000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | GAGAAGAGAAAATGA | 1500            |
| Sequence 2 | AAGCAAACAAAATAA | 1500            |
| Sequence 3 | GAGCAAACAAAATAA | 1500            |
| Sequence 4 | GAGAAAGGAAAAAAA | 1500            |
| Sequence 5 | TAGAAGAGAAGGAAA | 1500            |
| Sequence 6 | GAAAACACAAAAAGA | 1500            |
| Sequence 7 | GAGAAGACACAATAA | 1500            |
| Sequence 8 | TAGTAAGTAAAATAA | 1500            |
| Sequence 9 | AAAAAAAAAAAAAGA | 1500            |
| Sequence 10| GAGCTCAGAAAATGA | 1500            |

**Entropy of the generated motifs:** 1.4227919097643442

## Sample run on yst04r

- **Number of sequences available:** 7
- **Length of k-mer:** 10
- **Number of iterations:** 10000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TTCTGGAATG    | 1000            |
| Sequence 2 | TTCTGGCATC    | 1000            |
| Sequence 3 | TTCTGGAACA    | 1000            |
| Sequence 4 | TTCTGGCAAC    | 1000            |
| Sequence 5 | TTCTGGCACA    | 1000            |
| Sequence 6 | AACTGGCATC    | 1000            |
| Sequence 7 | TTCCGGCAAG    | 1000            |

**Entropy of the generated motifs:** 1.493625565197716


- **Number of sequences available:** 7
- **Length of k-mer:** 5
- **Number of iterations:** 1000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TCCTA         | 1000            |
| Sequence 2 | TCCTA         | 1000            |
| Sequence 3 | TGCTA         | 1000            |
| Sequence 4 | TCCTA         | 1000            |
| Sequence 5 | TCCTA         | 1000            |
| Sequence 6 | TCCTA         | 1000            |
| Sequence 7 | TCCTA         | 1000            |

**Entropy of the generated motifs:** 1.3203137194663295


- **Number of sequences available:** 7
- **Length of k-mer:** 15
- **Number of iterations:** 1000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | TTGCAAAAAGAACAA | 1000            |
| Sequence 2 | TTTCCAAAAAATCAA | 1000            |
| Sequence 3 | TAGGAAAAGAAAAAA | 1000            |
| Sequence 4 | TTTGAAATAAAAAAA | 1000            |
| Sequence 5 | TTTCATAAAAAACCA | 1000            |
| Sequence 6 | ATATAAAAAAAAAAA | 1000            |
| Sequence 7 | TTCCTAAAAAAAAAA | 1000            |

**Entropy of the generated motifs:** 1.5233667301963683

## Sample run on yst08r

- **Number of sequences available:** 11
- **Length of k-mer:** 10
- **Number of iterations:** 10000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | AAAAAAGAAA    | 1000            |
| Sequence 2 | AAAAAAAAAA    | 1000            |
| Sequence 3 | GAAAAAAAAA    | 1000            |
| Sequence 4 | AAAAAAAAAA    | 1000            |
| Sequence 5 | AAAAAAGAAA    | 1000            |
| Sequence 6 | CAATAACAAA    | 1000            |
| Sequence 7 | AAAGAAAAAA    | 1000            |
| Sequence 8 | AAAAAAAAAA    | 1000            |
| Sequence 9 | AAAAAAAAAA    | 1000            |
| Sequence 10| AAATATAAAA    | 1000            |
| Sequence 11| AAAAAATCAA    | 1000            |

**Entropy of the generated motifs:** 1.2371330848120432


- **Number of sequences available:** 11
- **Length of k-mer:** 5
- **Number of iterations:** 1000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | AAGGT         | 1000            |
| Sequence 2 | AAGAT         | 1000            |
| Sequence 3 | AAGAT         | 1000            |
| Sequence 4 | AAGAT         | 1000            |
| Sequence 5 | AAGTT         | 1000            |
| Sequence 6 | AAGAT         | 1000            |
| Sequence 7 | AAGAT         | 1000            |
| Sequence 8 | AAGAT         | 1000            |
| Sequence 9 | AAGAT         | 1000            |
| Sequence 10| AAGAT         | 1000            |
| Sequence 11| AAGAT         | 1000            |

**Entropy of the generated motifs:** 1.1162575158286636


- **Number of sequences available:** 11
- **Length of k-mer:** 15
- **Number of iterations:** 1000

### Motif Results

| Sequence   | Motif         | Sequence length |
|------------|---------------|-----------------|
| Sequence 1 | AAAAAAAAAGAAAAA | 1000            |
| Sequence 2 | TATATAAAAAAAAAA | 1000            |
| Sequence 3 | AAAAAAAATATATAA | 1000            |
| Sequence 4 | AAAAAAAAAAAAAAA | 1000            |
| Sequence 5 | TCAAAAAAGAAAAAA | 1000            |
| Sequence 6 | ACTAGCAATAACAAA | 1000            |
| Sequence 7 | AAAAGAAAAAAGAGA | 1000            |
| Sequence 8 | AAAAGAAAGAAAAAA | 1000            |
| Sequence 9 | AAAGTAAAAAAAAAA | 1000            |
| Sequence 10| ACAACAAATATAAAA | 1000            |
| Sequence 11| ACTACAAAAAACACA | 1000            |

**Entropy of the generated motifs:** 1.3673784865647722
