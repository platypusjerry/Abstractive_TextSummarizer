# Abstractive_TextSummarizer
A project to implement **LSTM** based **Seq2Seq Encoder-Decoder** model with **attention mechanism** to summarize lengthy articles.

The model was trained on **CNN / Daily Mail** dataset as processed by **Nallapati et al. (2016)**.The dataset contains online news articles (781 tokens on average) paired with multi-sentence summaries (3.75 sentences or 56 tokens on average). The processed version contains 287,226 training pairs, 13,368 validation pairs and 11,490 test pairs. Models are evaluated with BLEU score.

The **BLEU score** of **0.38** ws achieved on the model. <br />
Used pre-trained **GloVE** embedding vectors.
# Predictions

**Review:** amid crowning new world champion another dazzling performance amir khan las vegas strip witnessed yet farcical scoring saturday night end year blighted bad decisions ringside judges cosmopolitan hotel guilty yet glaring errors ireland s andy lee glad spared fate stopped matt korobov win wbo middleweight crown timothy bradley <br />
**Original summary:** mauricio herrera timothy bradley left stunned scores read bradley looked returned winning ways diego chaves three ringside judges saw fight differently draw bradley s promoter bob arum livid judgement herrera looked done enough edge jose benavidez herrera however also denied judges <br />
**Predicted summary:**  floyd mayweather manny pacquiao wbo welterweight title las vegas lawler saunders welterweight champion eubank jnr world champion amir khan fight

Predictions on the Inshorts dataset(https://github.com/sunnysai12345/News_Summary)

**Review:** delhi high court upheld trial court order granting anticipatory bail congress leader sajjan kumar alleged murder three sikhs 1984 riots pm indira gandhi assassination court noted special investigation team challenging trial court order make ground bail cancellation <br />
**Original summary:** hc upholds bail order cong leader accused 1984 riots <br />
**Predicted summary**:  hc upholds plea seeking death tandoor 1984 riots case  <br />

**Review:** grand mosque mecca set undergo 266 billion expansion nearly two years work stopped wake crane collapse site left 107 people dead development grand mosque surrounding area resume annual haj pilgrimage <br />
**Original summary:** saudi restart work 266 bn grand mosque expansion <br />
**Predicted summary:**  restart opens world largest largest demolished

# To get better predictions
1. Implement Beam Search for the decoder.
2. Use Bi-Directional LSTMs to capture the context from both side of the sequence. 
3. We can look for better attention mechanism.
4. Implement Transformer model.
