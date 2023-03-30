# cbt 
## chatgpt 
As an AI language model, I am not sure about the specific context of "cbt" command. However, CBT stands for "Computer-Based Training," which refers to any kind of learning or training that utilizes digital technology (such as a computer or mobile device) as the primary mode of delivery. CBT can encompass a wide range of educational content, including interactive videos, simulations, games, quizzes, and other multimedia materials. This type of training can be self-paced, allowing users to learn at their own speed and on their own schedule, and can be facilitated through a variety of platforms, including web-based applications, mobile apps, and learning management systems. It can also be useful for remote teams and online learning. 

## tldr 
 
> Utility for reading data from Google Cloud's Bigtable.
> More information: <https://cloud.google.com/bigtable/docs/cbt-reference>.

- List tables in the current project:

`cbt ls`

- Print count of rows in a specific table in the current project:

`cbt count "{{table_name}}"`

- Display a single row from a specific table with only 1 (most recent) cell revision per column in the current project:

`cbt lookup "{{table_name}}" "{{row_key}}" cells-per-column={{1}}`

- Display a single row with only specific column(s) (omit qualifier to return entire family) in the current project:

`cbt lookup "{{table_name}}" "{{row_key}}" columns="{{family1:qualifier1,family2:qualifier2,...}}"`

- Search up to 5 rows in the current project by a specific regex pattern and print them:

`cbt read "{{table_name}}" regex="{{row_key_pattern}}" count={{5}}`

- Read a specific range of rows and print only returned row keys in the current project:

`cbt read {{table_name}} start={{start_row_key}} end={{end_row_key}} keys-only=true`
