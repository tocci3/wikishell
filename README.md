# wikishell
A bash script for getting the lead sentence of Wikipedia artiles from command line.

Get xml data from Entligh Wikipedia API (https://en.wikipedia.org/w/api.php) or Japanese Wikipeida API (https://ja.wikipedia.org/w/api.php), extract a first sentence and remove markup tags.

## Usage
./wikishell [Options] <word>
  
|Option         | Description    |
|---------------|----------------|
|-j  --japanese |use japanese api|
|-h  --help     |display help    |

### example
```
$ ./wikishell football
Football is a family of team sports that involve, to varying degrees, kicking a ball to score a goal.  Unqualified, the word football is understood to refer to whichever form of football is the most popular in the regional context in which the word appears. Sports commonly called football in certain places include association football (known as soccer in some countries); gridiron football (specifically American football or Canadian football); Australian rules football; rugby football (either rugby league or rugby union); and Gaelic football. These different variations of football are known as football codes.
```

Use Japanese Wikipedia api
```
$ ./wikishell -j ラモス瑠偉
ラモス 瑠偉（ラモス ルイ、Ramos Ruy、1957年2月9日 - ）は、ブラジル・リオデジャネイロ出身の元サッカー選手、サッカー指導者（JFA 公認S級コーチ）、フットサル選手、タレントである。1989年に日本に帰化。長男はサッカー指導者のラモス・ファビアノ。長女は歌手のFABiANA。
```
