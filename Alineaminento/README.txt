
DECODIFICADOR DEEPSPEECH

1. Exportar modelo de DeepSpeech

En la carpeta /ASR/System/deepspeech/Euskara o Español ejecutar el script ./run.sh para entrenar un modelo y crearlo. 
Esto creará una carpeta /000 donde estara el modelo y los resultados del experimento. 
El modelo se llama output_graph.pb y se utiliza para decodificar el audio.

2. Decodificar audio

Para decodificar el audio en la carpeta /ASR/System/deepspeech/Alienamiento está el programa run.sh que necesita como argumento en nombre del audio que se quiera decodificar.
El audio tiene que estar en la misma carpeta que el script.
El script tiene como paramtros:

    --scorer El scorer que se utiliza para entrenar el modelo. /ASR/LM/EU/wikipedia.mini/deepspeech/kenlm.scorer
    --model El modelo que hemos creado
    --audio El audio que escribimos junto al programa.
    --json Parametro para que exporte el modelo JSON



    --candidate_transcripts 1 Cuantas transcripciones queremos que escriba.



Este script creara un archivo con formatu JSON que se visualizará de este modo.
