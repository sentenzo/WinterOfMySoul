# Определение видовой пренадлежности по ДНК

Узнать последовательность некоторого фрагмента ДНК это, конечно, здорово, но, просто взглянув на последовательность, можно не понять, а что это вообще за фрагмент, что в нем закодировано (и закодировано ли вообще?) и из какого организма этот фрагмент ДНК.

В этом задании мы узнаем, как ответить на последний вопрос.

Представим, что у вас есть фрагмент ДНК, вы его отсеквенировали и получили следующую последовательность:

    AAATTAACGAGTGTGAAAAATTGAAAACCTCTCTCTTTCTCATTTTCCCTTTTTTTCTCTTTATCTCAAG
    CTCATTCTTCTTCTTAATAACTAGATCTCTCTTTCTTTCTTCTTATTTTTCTCTTCTCTTCTTTAGTTTC
    GCTTATCTCGCGGCTCTGACCAGCTCTCAAGTTGTTCGTTTCTGGTTAATGGATATTGAACCCTCTTGGG
    ATCTTGGGGGGGTGGTTATTTCCTTTTCGAAATTGCATGGCAACATCAAATGACCAAACCAATACTAAAT
    CATCACATTCTCGTACTCTTCTCCTTCTCTTCATCTTCTTATCCCTCCTTCTCTTCAGTAGCCTTACAAT
    CCCCATGACTCGTCATCAGTCCACATCTATGGTTGCTCCCTTCAAGAGGGTTCTCCTCGAATCTTCAGTT
    CCAGCTTCATCAACAATGGATCTACGTCCAAAGGCTAGCACACGACGCAGCCGCACTTCTAGAAGGAGAG
    AGTTTGGAAATGATGCTCATGAGGTTCCTAGTGGTCCAAACCCTATTTCCAACTAGGTGAGTTGGCACAT
    CTGGTTTTTTACCGGTGAGTTTGAAAGATAAGTTATTATAGATCAATATTATATGTATATTTGAGAAGCT
    TCTGATCGATGGAGATCAGAGAGAAGCTTCATTATTATGGACTTTTTTTGGATATGAATTATCAAGAATT
    TGGTATATATTTCTTTGGATCGATCAATTTGGTACCATTCCATCTCCTTAAAATCTTTTGTTCGTTCTAA
    TATTGTTTTCTCCATCTATTAAGTTTTGAAGTTAGAAGTGTAAAGAAGAGATATATACTCTTTATTTATT
    CACATGTGACTGTGTGTATATGTAGCCACCTCTGCATTTCCTTCACAAAGTATTTGGGATATAGAATCTT
    TTATAATTGTTAGATTTGTCT
    
Для того чтобы определить, что это за фрагмент, воспользуемся инструментом под названием BLAST (Basic Local Alignment Search Tool) на сайте NCBI (The National Center for Biotechnology Information). Если вкратце, то это программа, которая ищет сходные последовательности ДНК в большой базе данных, где собрана информация о различных последовательностях ДНК. Если загрузить туда интересующий нас фрагмент, то мы сможем найти в этой базе наиболее похожие ДНК и на этом основании предполагать, из какого организма этот фрагмент ДНК и какие функции выполняет (если, конечно, в базе есть что-то похожее).

Для решения задания необходимо:

1. Перейти по [ссылке](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PROGRAM=blastn&PAGE_TYPE=BlastSearch&LINK_LOC=blasthome)
2. Скопировать предложенную в задании последовательность в специальное окошко
3. Нажать BLAST

![blast_0](get/img/ru_0.md/i000.png)

Затем надо немного подождать, пока не появится страница примерно такого вида:

![blast_0](get/img/ru_0.md/i001.png)

Затем нужно промотать страницу вниз до раздела Alignments. Посмотреть на верхний результат и скопировать латинское название организма, из генома которого взят предложенный фрагмент ДНК (это будут первые два слова).

Ответ должен выглядеть примерно так:

    Canis lupus