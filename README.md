# ascii-convert-mysql-function

This function is used to convert the ascii characters corresponding to the Turkish characters in the strings held in the ascii MySQL database to Turkish characters. It is used to translate ascii equivalents of <,>, ",", &, and space characters besides Ş, ş, Ç, ç, İ, ı, Ö, ö, Ü, ü,
You can change and use it by yourself. I hope it helps.

# Sample Usage;
select text from posts

& lt; p & gt; & lt; strong & gt; International & amp; nbsp; Treaties & amp; nbsp; authorizations and publishing rights belong to: & lt; p & gt;

select FTURKCE(text) from posts
<p> <strong> Which of the following do you have the authority to approve and publish international agreements? </ strong> </ p>
