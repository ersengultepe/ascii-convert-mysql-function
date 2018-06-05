# ascii-convert-mysql-function

This function is used to convert the ascii characters corresponding to the Turkish characters in the strings held in the ascii MySQL database to Turkish characters. It is used to translate ascii equivalents of <,>, ",", &, and space characters besides Ş, ş, Ç, ç, İ, ı, Ö, ö, Ü, ü,
You can change and use it by yourself. I hope it helps.

# Sample Usage;

without using functions
select text from posts
&lt;p&gt;&lt;strong&gt;Milletlerarası&amp;nbsp;andlaşmaları&amp;nbsp;onaylama ve yayımlama yetkisi aşağıdakilerden hangisine aittir?&lt;/strong&gt;&lt;/p&gt;

after using the function
select FTURKCE(text) from posts
<p><strong>Milletlerarası andlaşmaları onaylama ve yayımlama yetkisi aşağıdakilerden hangisine aittir?</strong></p>
