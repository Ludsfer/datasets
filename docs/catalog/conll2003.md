<div itemscope itemtype="http://schema.org/Dataset">
  <div itemscope itemprop="includedInDataCatalog" itemtype="http://schema.org/DataCatalog">
    <meta itemprop="name" content="TensorFlow Datasets" />
  </div>
  <meta itemprop="name" content="conll2003" />
  <meta itemprop="description" content="Example of a CoNLL-formatted dataset.&#10;&#10;To use this dataset:&#10;&#10;```python&#10;import tensorflow_datasets as tfds&#10;&#10;ds = tfds.load(&#x27;conll2003&#x27;, split=&#x27;train&#x27;)&#10;for ex in ds.take(4):&#10;  print(ex)&#10;```&#10;&#10;See [the guide](https://www.tensorflow.org/datasets/overview) for more&#10;informations on [tensorflow_datasets](https://www.tensorflow.org/datasets).&#10;&#10;" />
  <meta itemprop="url" content="https://www.tensorflow.org/datasets/catalog/conll2003" />
  <meta itemprop="sameAs" content="https://www.aclweb.org/anthology/W03-0419/" />
  <meta itemprop="citation" content="@inproceedings{tjong-kim-sang-de-meulder-2003-introduction,&#10;    title = &quot;Introduction to the {C}o{NLL}-2003 Shared Task: Language-Independent Named Entity Recognition&quot;,&#10;    author = &quot;Tjong Kim Sang, Erik F.  and&#10;      De Meulder, Fien&quot;,&#10;    booktitle = &quot;Proceedings of the Seventh Conference on Natural Language Learning at {HLT}-{NAACL} 2003&quot;,&#10;    year = &quot;2003&quot;,&#10;    url = &quot;https://www.aclweb.org/anthology/W03-0419&quot;,&#10;    pages = &quot;142--147&quot;,&#10;}" />
</div>

# `conll2003`


Note: This dataset was added recently and is only available in our
`tfds-nightly` package
<span class="material-icons" title="Available only in the tfds-nightly package">nights_stay</span>.

*   **Description**:

Example of a CoNLL-formatted dataset.

*   **Homepage**:
    [https://www.aclweb.org/anthology/W03-0419/](https://www.aclweb.org/anthology/W03-0419/)

*   **Source code**:
    [`tfds.text.conll2003.Conll2003`](https://github.com/tensorflow/datasets/tree/master/tensorflow_datasets/text/conll2003/conll2003.py)

*   **Versions**:

    *   **`1.0.0`** (default): Initial release.

*   **Download size**: `959.94 KiB`

*   **Dataset size**: `3.87 MiB`

*   **Auto-cached**
    ([documentation](https://www.tensorflow.org/datasets/performances#auto-caching)):
    Yes

*   **Splits**:

Split     | Examples
:-------- | -------:
`'dev'`   | 3,251
`'test'`  | 3,454
`'train'` | 14,042

*   **Feature structure**:

```python
FeaturesDict({
    'chunks': Sequence(ClassLabel(shape=(), dtype=tf.int64, num_classes=23)),
    'ner': Sequence(ClassLabel(shape=(), dtype=tf.int64, num_classes=9)),
    'pos': Sequence(ClassLabel(shape=(), dtype=tf.int64, num_classes=47)),
    'tokens': Sequence(Text(shape=(), dtype=tf.string)),
})
```

*   **Feature documentation**:

Feature | Class                | Shape   | Dtype     | Description
:------ | :------------------- | :------ | :-------- | :----------
        | FeaturesDict         |         |           |
chunks  | Sequence(ClassLabel) | (None,) | tf.int64  |
ner     | Sequence(ClassLabel) | (None,) | tf.int64  |
pos     | Sequence(ClassLabel) | (None,) | tf.int64  |
tokens  | Sequence(Text)       | (None,) | tf.string |

*   **Supervised keys** (See
    [`as_supervised` doc](https://www.tensorflow.org/datasets/api_docs/python/tfds/load#args)):
    `None`

*   **Figure**
    ([tfds.show_examples](https://www.tensorflow.org/datasets/api_docs/python/tfds/visualization/show_examples)):
    Not supported.

*   **Examples**
    ([tfds.as_dataframe](https://www.tensorflow.org/datasets/api_docs/python/tfds/as_dataframe)):

<!-- mdformat off(HTML should not be auto-formatted) -->

{% framebox %}

<button id="displaydataframe">Display examples...</button>
<div id="dataframecontent" style="overflow-x:auto"></div>
<script>
const url = "https://storage.googleapis.com/tfds-data/visualization/dataframe/conll2003-conll2022-1.0.0.html";
const dataButton = document.getElementById('displaydataframe');
dataButton.addEventListener('click', async () => {
  // Disable the button after clicking (dataframe loaded only once).
  dataButton.disabled = true;

  const contentPane = document.getElementById('dataframecontent');
  try {
    const response = await fetch(url);
    // Error response codes don't throw an error, so force an error to show
    // the error message.
    if (!response.ok) throw Error(response.statusText);

    const data = await response.text();
    contentPane.innerHTML = data;
  } catch (e) {
    contentPane.innerHTML =
        'Error loading examples. If the error persist, please open '
        + 'a new issue.';
  }
});
</script>

{% endframebox %}

<!-- mdformat on -->

*   **Citation**:

```
@inproceedings{tjong-kim-sang-de-meulder-2003-introduction,
    title = "Introduction to the {C}o{NLL}-2003 Shared Task: Language-Independent Named Entity Recognition",
    author = "Tjong Kim Sang, Erik F.  and
      De Meulder, Fien",
    booktitle = "Proceedings of the Seventh Conference on Natural Language Learning at {HLT}-{NAACL} 2003",
    year = "2003",
    url = "https://www.aclweb.org/anthology/W03-0419",
    pages = "142--147",
}
```


## conll2003/conll2022 (default config)
