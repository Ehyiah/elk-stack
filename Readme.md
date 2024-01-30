exporter un pipeline :
curl -X GET "localhost:9200/_ingest/pipeline/votre_nom_de_pipeline" > /var/www/votre_nom_de_pipeline.json

importer un pipeline
curl -X PUT "localhost:9200/_ingest/pipeline/votre_nom_de_pipeline" -H 'Content-Type: application/json' -d @votre_nom_de_pipeline.json


Les pipeline doivent avoir le nom spécifié dans le filebeat.yml => c'est a dire symfony et caddy
