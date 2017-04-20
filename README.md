### **NOTE:** [tensorflow/syntaxnet](https://github.com/tensorflow/models/tree/master/syntaxnet) now includes *Parsey Universal* that provides models for other languages, including Portuguese, available [here](https://github.com/tensorflow/models/blob/master/syntaxnet/g3doc/universal.md).

# syntaxnet-portuguese

A Portuguese language model for [syntaxnet](https://github.com/tensorflow/models/tree/master/syntaxnet),
treebank data used is available from [Universal Dependencies](http://universaldependencies.org/).

## Usage

Clone and build [syntaxnet](https://github.com/tensorflow/models/tree/master/syntaxnet), then:

    $ git clone git@github.com:nunorc/syntaxnet-portuguese.git
    $ cd syntaxnet-portuguese
    # edit test.sh to update your syntaxnet home directoy
    $ echo "A Maria tem razão."  | ./test.sh 
    (...)
    INFO:tensorflow:Read 1 documents
    Input: A Maria tem razão .
    Parse:
    tem VERB ROOT
     +-- Maria PROPN nsubj
     |   +-- A DET det
     +-- razão NOUN dobj
     +-- . PUNCT punct

## Acknowledgements

Thank you to tensorflow and syntaxnet developers and maintainers.

Thank you to Myungchul Shin for sharing his [test code](https://github.com/dsindex/syntaxnet).

