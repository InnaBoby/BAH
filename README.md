# BAH
#решение использует только открытые библиотеки
#все модели подгружаются автоматически

#зависимости

!pip install transformers
from transformers import pipeline, AutoTokenizer, EncoderDecoderModel

!pip install sentencepiece
import sentencepiece

import pandas as pd
import numpy as np

from tqdm import tqdm

import re

#исправление орфографических ошибок
!pip install pyaspeller
from pyaspeller import YandexSpeller

#убираем стоп-слова
import nltk
nltk.download('stopwords')
from nltk.corpus import stopwords

#лемматизация
!pip install pymorphy2
import pymorphy2

#для автоматической загрузки файлов
from google.colab import files
