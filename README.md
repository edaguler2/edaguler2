{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [],
   "source": [
    "from nltk.tokenize import sent_tokenize, word_tokenize"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "metadata": {},
   "outputs": [],
   "source": [
    "text = \"Alan Turing, İngiliz matematikçi, bilgisayar bilimcisi ve kriptolog. Bilgisayar biliminin kurucusu sayılır. Geliştirmiş oldugu Turing testi ile makinelerin ve bilgisayarların düşünme yetisine sahip olup olamayacakları konusunda bir kriter öne sürmüştür.\""
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "['Alan',\n",
       " 'Turing,',\n",
       " 'İngiliz',\n",
       " 'matematikçi,',\n",
       " 'bilgisayar',\n",
       " 'bilimcisi',\n",
       " 've',\n",
       " 'kriptolog.',\n",
       " 'Bilgisayar',\n",
       " 'biliminin',\n",
       " 'kurucusu',\n",
       " 'sayılır.',\n",
       " 'Geliştirmiş',\n",
       " 'oldugu',\n",
       " 'Turing',\n",
       " 'testi',\n",
       " 'ile',\n",
       " 'makinelerin',\n",
       " 've',\n",
       " 'bilgisayarların',\n",
       " 'düşünme',\n",
       " 'yetisine',\n",
       " 'sahip',\n",
       " 'olup',\n",
       " 'olamayacakları',\n",
       " 'konusunda',\n",
       " 'bir',\n",
       " 'kriter',\n",
       " 'öne',\n",
       " 'sürmüştür.']"
      ]
     },
     "execution_count": 3,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "text.split()"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "['Alan',\n",
       " 'Turing',\n",
       " ',',\n",
       " 'İngiliz',\n",
       " 'matematikçi',\n",
       " ',',\n",
       " 'bilgisayar',\n",
       " 'bilimcisi',\n",
       " 've',\n",
       " 'kriptolog',\n",
       " '.',\n",
       " 'Bilgisayar',\n",
       " 'biliminin',\n",
       " 'kurucusu',\n",
       " 'sayılır',\n",
       " '.',\n",
       " 'Geliştirmiş',\n",
       " 'oldugu',\n",
       " 'Turing',\n",
       " 'testi',\n",
       " 'ile',\n",
       " 'makinelerin',\n",
       " 've',\n",
       " 'bilgisayarların',\n",
       " 'düşünme',\n",
       " 'yetisine',\n",
       " 'sahip',\n",
       " 'olup',\n",
       " 'olamayacakları',\n",
       " 'konusunda',\n",
       " 'bir',\n",
       " 'kriter',\n",
       " 'öne',\n",
       " 'sürmüştür',\n",
       " '.']"
      ]
     },
     "execution_count": 4,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "word_tokenize(text)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "['Alan Turing, İngiliz matematikçi, bilgisayar bilimcisi ve kriptolog.',\n",
       " 'Bilgisayar biliminin kurucusu sayılır.',\n",
       " 'Geliştirmiş oldugu Turing testi ile makinelerin ve bilgisayarların düşünme yetisine sahip olup olamayacakları konusunda bir kriter öne sürmüştür.']"
      ]
     },
     "execution_count": 5,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "sent_tokenize(text)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "metadata": {},
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "Alan\n",
      "Turing\n",
      ",\n",
      "İngiliz\n",
      "matematikçi\n",
      ",\n",
      "bilgisayar\n",
      "bilimcisi\n",
      "ve\n",
      "kriptolog\n",
      ".\n",
      "Bilgisayar\n",
      "biliminin\n",
      "kurucusu\n",
      "sayılır\n",
      ".\n",
      "Geliştirmiş\n",
      "oldugu\n",
      "Turing\n",
      "testi\n",
      "ile\n",
      "makinelerin\n",
      "ve\n",
      "bilgisayarların\n",
      "düşünme\n",
      "yetisine\n",
      "sahip\n",
      "olup\n",
      "olamayacakları\n",
      "konusunda\n",
      "bir\n",
      "kriter\n",
      "öne\n",
      "sürmüştür\n",
      ".\n"
     ]
    }
   ],
   "source": [
    "for token in word_tokenize(text):\n",
    "    print(token)"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.6.5"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}

