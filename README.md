# Fatick Stemmer
## Description
<!--
&nbsp; is for one char space and
&emsp; is for one tab space
-->
Orginal Authors main focus was to program a light-weight library to determine a identical word for same type of inflected word as stem to run on any model. Currently, generated stems efficacy for Data analysis and NLP tasks is yet to be determined.

## Installation
>### Run the following  to install:
+ using git
```
git clone https://github.com/SaifurOWL/Bangla-stemmer-Usable-Variant-for-self.git
cd Bangla-stemmer-Usable-Variant-for-self
python setup.py install
```
+ for colab (cloning to colabs own drive)
```
!git clone https://github.com/SaifurOWL/Bangla-stemmer-Usable-Variant-for-self.git
%cd /content/Bangla-stemmer-Usable-Variant-for-self
!python setup.py install
```

## Usages

> __Example 01__:

>```python
>from bangla_stemmer.stemmer import stemmer
>wordlist = ['কবিরগুলিকে', 'আমাকে', 'নামাবার']
>stmr = stemmer.BanglaStemmer()
>stm = stmr.stem(word)
>print(stm)
>```
>`output:  ['কবির', 'আমা', 'নামা']`

<!-- -->

> __Example 01__:

>```python
>from bangla_stemmer.stemmer.stemmer import BanglaStemmer
>word = 'কবিরগুলিকে'
>stm = BanglaStemmer().stem(word)
>print(stm)
>```
>`output:  ['কবির', 'আমা', 'নামা']`

## Grammar Rule
The grammar rules applied here are based on the algorithm of [*Rafi Kamal*](https://github.com/rafi-kamal/Bangla-Stemmer). However some major and required modification has been made in this library in order to make it compatible with any model.
&emsp;

<span style="color:gray; font-size:20px; font-family:courier">*__Reference:__*</span>
<span style = "font-size:15px">&emsp;&emsp; __&#11153;__ [*BanglaKit*](https://github.com/banglakit/bengali-stemmer)</span>
