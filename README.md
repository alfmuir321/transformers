# Transformers

Transformers completely from scratch! This is a project I've worked on for a while, to try to build transformers completely from scatch (without using ML frameworks).

> encoder_transformer_numpy: an example of a very basic encoder-only transformer, using numpy only. Can be trained using SGD on a simple task, which is to classifiy a sequence as containing the 'special number' or not. No LayerNorm, residual connections, or batching, so can only be a max of 3-4 layers before training becomes too unstable.

> decoder_transformer_pytorch: an example of a decoder-only transformer built using PyTorch. This one can be trained on the 'tiny shakespeare' dataset, which is a text dataset containing shakespearean text. More complex, using RMSNorm, full MHA, residual connections, mini-batches, and AdamW.

> decoder_transformer_numpy: same architecture as decoder_transformer_pytorch (full MHA, RMSNorm, etc.), but implemented using only numpy! CuPy is used for training (basically GPU numpy). I have included my forward and backprop calculations (with the shapes of everything) if you want to try to implement it yourself!
