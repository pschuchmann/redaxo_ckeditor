# redaxo_ckeditor

*Angepasster Init des CKEditors 4 für [Redaxo 5](https://redaxo.org/). Kompatibilität für MBlock hergestellt. Basierend auf dem Addon CKEditor von RexDude.*

## Anleitung

Um den CKEditor 4 mit MForm und MBlock zu verwenden, reicht es die Datei *redaxo.js* aus dem assets Ordner zu übernehmen. Diese muss auf der eigenen Webseite in den assets/addons/ckeditor Ordner kopiert und die bereits vorhandene Datei überschrieben werden.

Der Aufruf in MForm/MBlock passiert nun beispielhaft wie folgt:

```
$mform->addTextAreaField("$id.0.textarea_content", array(
  'label'                 => 'Text',
  'class'                 => 'ckeditor',
  'data-ckeditor-profile' => 'lite',
  ));
```

Es kann jedes beliebige Profil aus dem Backend verwendet werden.

Im Repository ist die letzte veröffentlichte Version *4.11.3.1* vom *19. März 2019* von RexDude inklusive der bereits angepassten *redaxo.js* Datei.

[CKEditor auf redaxo.org](https://redaxo.org/download/addons/ckeditor/)

