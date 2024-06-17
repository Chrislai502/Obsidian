https://arxiv.org/pdf/2405.12213

![[octo.pdf]]

# OCTO
Octo model is engineered for flexibility and scalability.
- Natural Language and Goal Images

### Architecture

**Core Components:**

1. **Input Tokenizers:** Transform language instructions (`l`), goals (`g`), and observation sequences (`o1, ..., oH`) into tokens (`Tl`, `Tg`, `To`).
2. **Transformer Backbone:** Processes the tokens and generates embeddings (`el`, `eg`, `eo = T(Tl, Tg, To)`).
1. **Readout Heads:** Produce the desired outputs, i.e., actions (`a`).

**Transformer Backbone and Readout Heads:**
- **Modular Design:** Non-existent observation tokens are fully masked out, enabling the addition or removal of observations or tasks during finetuning.
- **Readout Tokens:** Inserted readout tokens (`TR,t`) attend to preceding observation and task tokens but are not attended by them. This design allows them to passively read and process internal embeddings.

## Training Details
Removed data based on the following:
- Lack of image stream
- Delta End-Effector control
Adapting to general Datasets:
- Datasets are weighed based on size
- Missing camera Channels are zero padded
- Gripper Action Spaces are aligned across datasets