# I'm a poet!
Н. В. Гоголь. Ревизор(N.V. Gogol.  Auditor) - https://ilibrary.ru/text/473/p.1/index.html

### Task :
You are given a list of roles as an array and a play script as a string. 

Each line of the play script is presented as follows: Role: lyrics.

The text can contain any characters.

Write a program that will group lines by role, number them, and
return the result as a ready-made text (see example). Each group is displayed in
as follows:

Role:
i) text
j) text2
...
== line feed ==

i and j are the line numbers in the script. Line indexing starts at one, display groups
follows according to the order of the roles. Line breaks between groups are required,
line breaks at the end of the text are not counted.

```
Sample Input:

roles:

["Городничий","Аммос Федорович", 
        "Артемий Филиппович", "Лука Лукич"];

textLines:

"Городничий: Я пригласил вас, господа, с тем, чтобы сообщить вам пренеприятное известие: к
нам едет ревизор.
    Аммос Федорович: Как ревизор?

    Артемий Филиппович: Как ревизор?

    Городничий: Ревизор из Петербурга, инкогнито. И еще с секретным предписаньем.

    Аммос Федорович: Вот те на!

    Артемий Филиппович: Вот не было заботы, так подай!

    Лука Лукич: Господи боже! еще и с секретным предписаньем!"

Sample Output:

Городничий:

1) Я пригласил вас, господа, с тем, чтобы сообщить вам пренеприятное известие: к нам едет
ревизор.

4) Ревизор из Петербурга, инкогнито. И еще с секретным предписаньем.

Аммос Федорович:
2) Как ревизор?

5) Вот те на!

Артемий Филиппович:
3) Как ревизор?

6) Вот не было заботы, так подай!

Лука Лукич:

7) Господи боже! еще и с секретным предписаньем!
```