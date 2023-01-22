# DialogueDiscourseParsing_from_Amillert_updated

К сожалению, некоторые zip-папки оказались слишком большими для загрузки в репозиторий. Их можно скачать отсюда: 

__Алгоритм действий:__

1. распаковать amillert-DialogueDiscourseParsing-master.zip; так получаем папку, в которой работаем

2. распаковать data.zip, GloVe-master.zip и glove.6B.100d.zip, получившиеся две папки и файл txt соответственно положить в amillert-... . 

3. вручную создать в amillert-... папку outputs

4. через терминал перейти в Ubuntu, далее - в локальную папку amillert-..., там: python ./data_pre.py ./data/s1-league1-game1/unannotated/ ./outputs/res.json
  (про data/s1-league1-game1 : можно попробовать файлы из других папок или из нескольких/всех папок (всего в data их 15); я не знаю, как подать терминалу на вход несколько 
  директорий так, чтобы он прошёлся по всем и записал результат в один итоговой файл)
  
5. там же: python3 main.py --train
